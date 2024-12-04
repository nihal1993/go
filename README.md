In Go, a name is exported if it begins with a capital letter. For example, Pizza is an exported name, as is Pi, which is exported from the math package.

pizza and pi do not start with a capital letter, so they are not exported.

When importing a package, you can refer only to its exported names. Any "unexported" names are not accessible from outside the package.

Run the code. Notice the error message.

To fix the error, rename math.pi to math.Pi and try it again.

Go folder structure
unplex/
├── go.mod         // Go module file
├── main/
│   └── hello.go   // main package, contains the main function
├── unplex/
│   └── unplex.go  // unplex package, contains other functions
└── utils/
    └── utils.go   // utils package, contains utility functions

