{
	// this will help us creat header garde in faster way using #ifndef, #define, #endif
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
	// globale declaration for our class in Orthodox Canonical Form
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
	// made easier for us to define the Orthodox Canonical Form function member with the filename name
	// as class name
	"Orthodox Canonical Form filename Template": {
        "prefix": "DefineOrthodoxCanonicalForm_Filename",
        "body": [
            "${TM_FILENAME_BASE}::${TM_FILENAME_BASE}()",
			"{",
			"",
			"}",
            "${TM_FILENAME_BASE}::~${TM_FILENAME_BASE}()"
			"{",
			"",
			"}",
			"${TM_FILENAME_BASE}::${TM_FILENAME_BASE}(const ${TM_FILENAME_BASE}& copy)",
			"{",
			"",
			"}",
			"${TM_FILENAME_BASE}& ${TM_FILENAME_BASE}::operator=(const ${TM_FILENAME_BASE}& obj)",
			"{",
			"",
			"}",
        ],
        "description": "Create a filename class template"
    }
}
