# A sample command-line

This is a sample command-line script written in bash. It demonstrates an easy way to account parameters and format a help screen.

## Missing parameters

```bash
[sorens | ~/src/sample-cli> ./sample-cli
try 'sample-cli --help' for more information
```

## Help

```bash
[sorens | ~/src/sample-cli> ./sample-cli --help

Usage: sample-cli [options...]

  -h,  --help                 display this help message                         
  -v,  --version              display the version                               
  --foo                       display 'foo'                                     
  -b,  --bar                  display 'bar'                                     
```

The standard help screen displays using a 30 character column.

## Help with long command names

```bash
[sorens | ~/src/sample-cli> ./sample-cli --help

Usage: sample-cli [options...]

  -h,  --help                    display this help message                         
  -v,  --version                 display the version                               
  --foo                          display 'foo'                                     
  -b,  --bar                     display 'bar'                                     
  -mc, --multi-command           demonstrate a command that takes multipe parameters
  -vl, --very-very-long-command  display a very long command                       
```

If you create a long detailed command name, the help column will begin two spaces after the end of the detailed command name.

## A legal option

```bash
[sorens | ~/src/sample-cli> ./sample-cli --foo
foo!
```

## An illegal option

```bash
[sorens | ~/src/sample-cli> ./sample-cli --nothing
unknown command '--nothing'
try 'sample-cli --help' for more information
```

## Multiple parameters in a command

```bash
[sorens | ~/src/sample-cli> ./sample-cli -mc --baz hi
multi-command triggered, baz: 'hi'
```