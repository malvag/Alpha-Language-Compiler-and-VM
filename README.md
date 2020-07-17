# Alpha-Language-Compiler-and-VM

![Build](https://github.com/malvagos/Alpha-Language-Compiler-and-VM/workflows/Build/badge.svg)
#### Implementation of Alpha's compiler in 5 stages. ####
- Lexicographic analysis (yylex)
- Grammar and syntax construction (yacc - bison)
- Intermediate code and quad generation (library in c)
- Final code generation
- Construction of Alpha's virtual machine (AVM)

#### Usage:
```sh
        $ make {(empty)|out|avm_exec|clean}:
                - (empty)      : clean up, then build out and avm_exec
                - out          : alpha language compiler compilation recipe
                - avm_exec     : alpha language virtual machine executable compilation recipe
                - clean        : clean every executable and object
```
#### Compiles and returns a binary file at given location with .abc extension.
```sh
        $ ./out {file_path}
```
#### Runs the given file
```sh
        $ ./avm_exec {file_path}
```