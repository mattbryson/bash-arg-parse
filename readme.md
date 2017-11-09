# Bash Arg Parse Example
A simple bash script that can parse named, short and positional CLI arguments.

This is to be used as a template for simple bash scripts that accept various CLI arguments.

# Usage
Use `arg_parse_example` as the basis of a bash cli script.

To run the example...

````bash
$ ./arg_parse_example -h
usage: arg_parse_example -a AN_ARG -s SOME_MORE_ARGS [-y YET_MORE_ARGS || -h]

  -a | --an_arg            : The path to the original ipa file to be resigned
  -s | --some_more_args    : The path to the provisioning profile
  -y | --yet_more_args     : The identiy/name of the signing certifiate installed in keychain
  -h | --help              : This message
````



````bash
$ ./arg_parse_example -a foo --some_more_args bar one two
you passed in...

positional arg 1: one
positional arg 2: two
named arg: an_arg: foo
named arg: some_more_args: bar
named arg: yet_more_args: a default value
````
