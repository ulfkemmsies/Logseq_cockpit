- Query language used by [[Neo4j]]
- Learning from course at Graph Academy
	- MATCH for retrieving data
	- WHERE for creating conditions for matching
	- exists() for conditional checking
	- IS (NOT) NULL for property existence checking
	- STARTS WITH, ENDS WITH, CONTAINS for substring searches -> case sensitive
	- WHERE x IN [...] to find properties contained in list
	- MERGE to create new nodes, relationships after checking whether an instance with the same properties already exists
		- CREATE to do the same without checking, allows for multiple copies of exact same object
		- Label and primary property-value pair that defines it (e.g. name or title)
	- SET and REMOVE (or SET to NULL) to manipulate properties
	- ON CREATE and ON MATCH to do stuff automatically
	- Always separate node and relationship creation in MERGE
		- If one of two nodes already exists, error will occur
	- You cannot delete connected nodes, use DETACH DELETE instead to delete all connected edges first
		- MATCH (n) DETACH DELETE n to delete entire graph
	-
	-