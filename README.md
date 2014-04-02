J% - An Extensible Java Compiler 
========

Introduction
-------
J% (pronounced j-mod) is a DSL-aware (Domain-Specific Language) extension of the Java programming language. The prototype implementation consists of a preprocessor, which translates the J% source code to Java compatible code and finally compiles it, through <code>javac</code> to Java bytecode.

So far, it facilitates existing Java DSL APIs, like JDBC for SQL. But this is optional, a module can literally translate DSL code to the host language, since with J% any DSL can be easily integrated into the compiler infrastructure, act as a module and be initialized when needed.

Usage
-----
J% consists of a compiler (<code>jmodc</code>), which can be used to compile the source code.

	$ jmodc
	J% (aka J-mod) compiler
	-----------------------
	Vassilios Karakoidas (bkarak@aueb.gr)
	website: http://bkarak.wizhut.com/projects/jmod

	No options are given
	jmod compiler usage:
	jmod [switches] [files]

	options:
	-cc, --compiler-context : Prints current compiler context
	-st, --symbol-table : Export Symbol Table
	-h, --help : Displays help information
	-pextc, --print-external-context : Print the External context for each module call
	-i, --input-dir : Input source directories. use: input-dir1,input-dir2,...
	-cl, --compiler-list : Prints the available compiler list (back-ends)
	-am, --add-modules : Add thirs party external modules
	-wd, --work-dir : Define the working directory
	-pc, --print-classpath : Prints current classpath
	-mc, --metrics : Calculate basic metrics set of metrics
	-xml, --output-xml : Compiler output is set in XML
	-uext, --user-external : Print user-defined external type list
	-uexth, --user-external-helper : Print user-defined constructor helper
	-ml, --module-list : Prints the available External modules

Examples
-------
Several ported applications and several other experinments with can be found in [jmod-ports](https://github.com/bkarak/jmod-ports) repository.

Publications
-------

* Vassilios Karakoidas, Diomidis Spinellis, J%: Integrating Domain Specific Languages with Java, in _Proceedings of 13th Panhelenic Conference on Informatics (PCI 2009)_, pp. 109-113, 2009. [Download](http://bkarak.wizhut.com/www/pubs/pdfs/jmod-pci09.pdf)
