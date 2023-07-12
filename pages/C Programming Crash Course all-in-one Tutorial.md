type:: yt-video
link:: https://www.youtube.com/watch?v=1uR4tL-OSNI
tags:: programming

- ___
- {{video https://www.youtube.com/watch?v=1uR4tL-OSNI}}
	- {{youtube-timestamp 274}} C is a compiled language, the code gets compiled to an executable
	- {{youtube-timestamp 280}} All the syntax must be legal at compilation time
	- {{youtube-timestamp 319}} C is statically typed, must choose data type for variable at compile time
	- {{youtube-timestamp 457}} Terminal commands
	  collapsed:: true
		- {{youtube-timestamp 493}} ``pwd`` : absolute path
		- {{youtube-timestamp 517}} ``ls`` : list
		- {{youtube-timestamp 538}} Terminal flags e.g. ``ls -l`` is long list ``ls -a`` is all items
		- {{youtube-timestamp 560}} ``.`` : current directory
		- {{youtube-timestamp 569}} ``..`` : parent directory
		- {{youtube-timestamp 675}} ``~`` references the home directory
		- {{youtube-timestamp 709}} Can use ``../..`` to move up two parents
		- {{youtube-timestamp 743}} ``clear`` : clear window
		- {{youtube-timestamp 769}} ``touch`` : creates a file without any content
		- {{youtube-timestamp 802}} ``mv`` : move file
		- {{youtube-timestamp 829}} ``mkdir`` : make directory
		- {{youtube-timestamp 855}} ``rm`` : remove (-r for directory)
		- {{youtube-timestamp 902}} ``echo`` : print given string
		- {{youtube-timestamp 919}} Direct echo content to write to file using > e.g. ``echo "Hello" > filename``
		- {{youtube-timestamp 932}} ``cat`` : view or create file
		- {{youtube-timestamp 996}} ``less`` : allows you to scroll through file, exit with ``q``
		-
	- {{youtube-timestamp 1091}} Similar shell for all C programs
	- {{youtube-timestamp 1105}} `#include <file>` : equivalent of import
	- {{youtube-timestamp 1179}} Use `gcc -o filename` to compile file to filename executable
	- {{youtube-timestamp 1273}} Any change to code can only be reflected if recompiled
	- {{youtube-timestamp 1349}} Declaration and initialization of variables are separate
	  ``int y;
	  y = 10;``
	- {{youtube-timestamp 1388}} Format strings to parametrize strings
	  `printf("%s World", "Hello") = "Hello World"`
	- {{youtube-timestamp 1472}} Format string with `%d` to include numbers?
	- {{youtube-timestamp 1568}} Get user input with `scanf()` e.g. `scanf("%d", &varname)`
	  Must give the pointer to variable in order to change it!
	- {{youtube-timestamp 1647}} `&` prefix is 'address of operator' some variable that must be appended whenever changing a variable's value e.g. `&x`
	- tl
	-