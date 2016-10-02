```c
Usage: java -jar yuicompressor-2.4.8.jar [options] [input file]

Global Options
  -V, --version             Print version information
  -h, --help                Displays this information
  --type <js|css>           Specifies the type of the input file
  --charset <charset>       Read the input file using <charset>
  --line-break <column>     Insert a line break after the specified column number
  -v, --verbose             Display informational messages and warnings
  -o <file>                 Place the output into <file>. Defaults to stdout.
                            Multiple files can be processed using the following syntax:
                            java -jar yuicompressor.jar -o '.css$:-min.css' *.css
                            java -jar yuicompressor.jar -o '.js$:-min.js' *.js

JavaScript Options
  --nomunge                 Minify only, do not obfuscate
  --preserve-semi           Preserve all semicolons
  --disable-optimizations   Disable all micro optimizations
```
