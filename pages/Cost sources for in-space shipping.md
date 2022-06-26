- Contributing cost factors per trip:
	- Paying off initial vehicle manufacturing cost
	- Maintenance for damage and repairs
	- Cost of propellant
	- Infrastructural node facility use (both origin and target)
- In order to calculate cost contribution without knowing total mass shipped (this would need discrete event simulation), we must calculate contributions with trajectory variables
	- Each vehicle has an engine which has a total burn lifetime
		- If vehicles cannot have their engines switched out, then the engine lifetime is the vehicle's lifetime
		- If engines can be swapped, then both the engine and the total vehicle lifetime must be known
	- Each trajectory-vehicle combination yields a specific burn time
	- Each trajectory-vehicle combination yields a total transfer time assuming Hohmann transfers (these can also be consulted from pre-calculated tables)
	- The engine's contribution to the cost is its lifetime divided by the trip's burn time
		- The burn time is calculated using the vehicle's initial total [[Thrust-to-Mass Ratio]], Specific Impulse, and the trajectory's delta v
	- The vehicle's contribution to the cost is its lifetime divided by the trip's transfer time (if engines can be swapped)
	- The repair and maintenance cost has a constant and variable part
		- The constant is just the per-trip repair (e.g. from re-igniting engines)
			- This is a usually a fraction of the total initial cost
		- The variable part depends on the transfer time and total burn time
			- Examples: radiation exposure, subsystem operational time)
			- This is a fraction of the constant part
		- The coefficients that scale these contributions could be defined globally or per vehicle
			- First define globally, and if an instance value exists, use that
- Total equation for price-insensitive costs:
  $$C_{init} \cdot \frac{t_{burn}}{t_{life}} + P_{best} \cdot m_{prop} + C_{init} \cdot r_{repair} + C_{init} 
  \cdot r_{repair} \cdot f_{repair,var} \cdot \Delta V $$
  $$C_{init} \cdot ( \frac{t_{burn}}{t_{life}} + r_{repair} \cdot (1 + f_{repair, var} \cdot \Delta V ) )$$
  $$ $$
- Repair-specific costs:
  $$C_{repair} = C_{init} \cdot f_{repair} \cdot (1 + f_{repair, var} \cdot \Delta V) \cdot [\phi \cdot m_{init}(\Delta V) + \lambda \cdot m_{prop}(\Delta V)]$$
- Total new price expression:
  $$P_{new} = (C_{init} \cdot ( \frac{t_{burn}}{t_{life}} + r_{repair} \cdot (1 + f_{repair, var} \cdot \Delta V ) ) + P_{best} \cdot m_{prop} + P_{pay} \cdot m_{pay} ) \cdot \frac{1}{m_{pay}} \cdot f_{profit} $$
	- $T_{burn}$ has $M{init} in the numerator and thus cancels out to the known factor $m_{pay}/m_{init}$
		- This requires us to know the engine thrust in vacuum
	- In order to solve this using known factors, we can define $r_{repair}$ as a function of $m_{dry}$
		- This could make intuitive sense due to more dry mass meaning more system complexity and scale, and thus more repairs needed over time
		- By expressing dry mass using Sorensen's [[Gross-Sensitive Mass Term]] and [[Propellant-Sensitive Mass Term]], we can express the cost using only previously known factors
		  $$ r_{repair} = f_{repair} \cdot m_{dry}$$
		  $$ r_{repair} = f_{repair} \cdot  (\phi \cdot m_{init} + \lambda \cdot m_{prop})$$
	- So, the values that must be defined for the vehicle are:
	  $$\{ C_{init}, \quad T_{life}, \quad I_{sp}, \quad F_{T, eng}, \quad \phi, \quad \lambda, \quad  f_{repair}, \quad f_{repair, var} \}$$
	  where the engine/propellant combination supplies
	  $$ \{ T_{life}, \quad I_{sp}, \quad F_{T, eng}  \} \rightarrow \{ \phi, \quad \lambda \}$$
	- Per trajectory, the following quantities must be known:
	  $$ \{ \Delta V, \quad f_{profit} \}$$
	- Per node, the following must be known:
	  $$ \{ P_{best}, \quad P_{pay} \}$$