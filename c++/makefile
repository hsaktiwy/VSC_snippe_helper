{
	// Place your snippets for makefile here. Each snippet is defined under a snippet name and has a prefix, body and 
	// description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
	// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the 
	// same ids are connected.
	// Example:
	// "Print to console": {
	// 	"prefix": "log",
	// 	"body": [
	// 		"console.log('$1');",
	// 		"$2"
	// 	],
	// 	"description": "Log output to console"
	// }
	"Defaultc++98": {
		"prefix": "Default",
		"body": [
			"C = c++",
			"flag = -Wall -Wextra -Werror -std=c++98",
			"src = ",
			"obj = $(src:.cpp=.o)",
			"Name = a.out",
			"all : $(Name)",
			"",
			"$(Name) : $(obj)"
        	"	$(C) $(obj) -o $@"
			"%.o : %.cpp",
			"		$(C) $(flag) -c $< -o $@",
			"clean:",
			"		rm -f $(obj)",
			"fclean: clean",
			"		rm -f $(Name)",
			"re: fclean all",
			"",
			".PHONY: re fclean all clean"
		],
		"description": "default body off makefile"
	}
}