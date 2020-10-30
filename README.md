# csv2fhir
A tool to convert a bunch of .csv data files into a FHIR® bundle.

## Requirements
Save all the worksheets in the excelsheet as .csv in one folder.
Provide this folder as input directory for the application.
## Usage

### Download
If not done already download git repository and build the jar as follows:
```bash
git clone https://github.com/life-research/csv2fhir.git
cd csv2fhir/
mvn package
cd target/

```
### Use
Now you can run the application like so:
```bash
java -jar csv2fhir-1.0-SNAPSHOT-jar-with-dependencies.jar -i INPUT-DIRECTORY -o OUTPUT-FILE 
```

If you need help run:
```
java -jar csv2fhir-1.0-SNAPSHOT-jar-with-dependencies.jar -h
```
output:
```
Usage: csv2fhir [-hV] -i=INPUT-DIRECTORY -o=OUTPUT-FILE
Converts a directory containing multiple csv files into a json bundle.
  -h, --help      Show this help message and exit.
  -i, --input-directory=INPUT-DIRECTORY
                  supply the input Directory here
  -o, --output-file=OUTPUT-FILE
                  supply the output File here
  -V, --version   Print version information and exit.
```
