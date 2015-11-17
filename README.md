# Java4selenium_template(j4s_template)

License: [MIT](License.txt)

This is console applications.

## Usage

### build fat jar

> gradle fatJar

### run with jar

java -jar *.jar [-options]

where oprions include:
*    -browser, -b <value>     	   set browser to test - 'FIREFOX' is default. ('FIREFOX','CHROME','OPERA','SAFARI','IE')
*    -all                          select all existing tests to execute.
*    -groups, -g <args...> 	   specifies list of groups of tests to execute.
*    -tests, -t <args...>  	   specifies list of tests to execute
*    -test_list, -tl	   	   print list of existing tests
*    -stop_on_error, -s	   	   if specified, tests will be stopper after first error
*    -help_g, -hg		   print help message for gradle
*    -help, -h                 	   print help message for jar

## Example

### call help

> java -jar *.jar -help

### run all tests

> java -jar *.jar -all

### run custom groups of tests on custom browser

> java -jar  *.jar -browser="OPERA" -groups GoogleGroup JiraGroup

### run custom group of tests and list of tests

> java -jar *.jar -groups GoogleGroup -tests JiraLoginTest JiraLoguotTest2

