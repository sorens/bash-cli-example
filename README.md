# A sample command-line

This is a sample command-line script written in bash. It demonstrates an easy way to account parameters and format a help screen.

```bash
[sorens | ~/src/sample-cli> ./sample-cli
try 'sample-cli --help' for more information
[sorens | ~/src/sample-cli> ./sample-cli --help

Usage: sample-cli [options...]

  -h,  --help                         display this help message                         
  -v,  --version                      display the version                               
  --foo                               display 'foo'                                     
  -b,  --bar                          display 'bar'                                     
  -vl, --very-very-long-long-command  display a very long command                       
[sorens | ~/src/sample-cli> ./sample-cli --foo
foo!
[sorens | ~/src/sample-cli> ./sample-cli -r
unknown command
try 'sample-cli --help' for more information
[sorens | ~/src/sample-cli> 
```