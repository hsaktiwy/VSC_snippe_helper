{
	// This will help us create header guards in faster way using #ifndef, #define, #endif
	"Header Guard": {
		"prefix": "hdr",
		"body": [
			"#ifndef ${TM_FILENAME_BASE/(.*)/${1:/upcase}/}_HPP",
			"#define ${TM_FILENAME_BASE/(.*)/${1:/upcase}/}_HPP",
			"",
			"#endif"
		],
		"description": "Header Guard"
	},
	// To display the file name
	"File Name Display": {
		"prefix": "fn",
		"body": [
			"${TM_FILENAME_BASE}",
		],
		"description": "Write file name"
	},
	// Globale declaration for our class in Orthodox Canonical Form
	"Class Globale Template": {
        "prefix": "GClassT",
        "body": [
            "class $1 {",
			"    public:",
            "    	$1();",
            "    	~$1();",
			"    	$1(const $1& copy);",
			"    	$1& operator=(const $1& obj);",
            "}",
        ],
        "description": "Create a Globale class template"
    },
	// declaration for our class named as the same as the filename in Orthodox Canonical Form
	"Class filename Template": {
        "prefix": "FileClassT",
        "body": [
            "class ${TM_FILENAME_BASE} {",
			"    public:",
            "    	${TM_FILENAME_BASE}();",
            "    	~${TM_FILENAME_BASE}();",
			"    	${TM_FILENAME_BASE}(const ${TM_FILENAME_BASE}& copy);",
			"    	${TM_FILENAME_BASE}& operator=(const ${TM_FILENAME_BASE}& obj);",
            "};",
        ],
        "description": "Create a filename class template"
    },
	"Empty Class filename Template": {
        "prefix": "EmptyFileClassT",
        "body": [
            "class ${TM_FILENAME_BASE} {",
			"",
            "};",
        ],
        "description": "Create a Empty filename class template"
    },
	// Made easier for us to define the Orthodox Canonical Form functions member with the filename name
	// as class name
	"Orthodox Canonical Form filename Template": {
        "prefix": "DefineOrthodoxCanonicalForm_Filename",
        "body": [
			"#include \"${TM_FILENAME_BASE}.hpp\"",
			"",
            "${TM_FILENAME_BASE}::${TM_FILENAME_BASE}()",
			"{",
			"",
			"}",
			"",
            "${TM_FILENAME_BASE}::~${TM_FILENAME_BASE}()"
			"{",
			"",
			"}",
			"",
			"${TM_FILENAME_BASE}::${TM_FILENAME_BASE}(const ${TM_FILENAME_BASE}& copy)",
			"{",
			"	*this = copy;",
			"}",
			"",
			"${TM_FILENAME_BASE}& ${TM_FILENAME_BASE}::operator=(const ${TM_FILENAME_BASE}& obj)",
			"{",
			"	if (this != &obj)",
			"	{",
			"",
			"	}",
			"	return (*this);"
			"}",
        ],
        "description": "Create a filename class template"
    },
	// to display std::endl
	"New line": {
		"prefix": "endl",
		"body": [
			"std::endl;",
		],
		"description": "right std::endl"
	},
	// just to make thing faster
	"cout shortcut":{
		"prefix": "cout",
		"body":[
			"std::cout << $1 << std::endl;",
		],
		"description": "cout quick display"
	},
	"cerr shortcut":{
		"prefix": "cerr",
		"body":[
			"std::cerr << \"$1\" << std::endl;",
		],
		"description": "cerr quick display"
	},
	//And i create this cause i hate to write it when i need it in my test main.cpp
	"Display divider1":{
		"prefix": "DD1",
		"body":[
			"std::cout << \"////////////////////////////////////////////////////////////\" << std::endl;",
		],
		"description": "print that will devide the display using cout"
	},
	// this will make our header file creation much faster 
	"Headerfile ":{
		"prefix": "HDRCLASS",
		"body":[
			"#ifndef ${TM_FILENAME_BASE/(.*)/${1:/upcase}/}_HPP",
			"#define ${TM_FILENAME_BASE/(.*)/${1:/upcase}/}_HPP",
			"class ${TM_FILENAME_BASE} {",
			"    public:",
            "    	${TM_FILENAME_BASE}();",
            "    	~${TM_FILENAME_BASE}();",
			"    	${TM_FILENAME_BASE}(const ${TM_FILENAME_BASE}& copy);",
			"    	${TM_FILENAME_BASE}& operator=(const ${TM_FILENAME_BASE}& obj);",
            "};",
			"",
			"#endif"
		],
		"description": "print that will devide the display using cout"
	},
	"Default main":{
		"prefix": "Default",
		"body":[
			"int main(int argc, char **argv)",
			"{",
			"",
			"	return (0);",
			"}",
		],
		"description": "print that will devide the display using cout"
	},
	"Template delaration":{
		"prefix": "Template",
		"body":[
			"template <typename T>",
		],
		"description": "This is a template declaration or header"
	},
	"Template function":{
		"prefix": "TemplateFunction",
		"body":[
			"template <typename T> $1()",
			"{",
			"",
			"}",
		],
		"description": "Default template function module"
	},
	"Create Exception Class":{
		"prefix": "ExceptionClass",
		"body":[
			"#include <exception>",
			"class $1 : public std::exception",
			"{",
			"	const char *what() const throw()",
			"	{",
			"		return (\"$2\");"
			"	}",
			"};",
		],
		"description": "Default template function module"
	},
	"leaks test using leaks command in macos only C/C++":{
		"prefix": "LeaksMacosFunction_C/C++",
		"body":[
			"void leaks( void )",
			"{",
			"	system(\"leaks $1\");",
			"};",
		],
		"description": "leaks test using leaks command in macos only C/C++"
	},
}
