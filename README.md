# CSV-to-XES Project
This Java project is able to convert CSV-files into XES-files, the XML-based standard for process mining applications.

Forked from s41m1r. 

I tweaked the project such that it accepts an input directory and output directory. 
The input directory is a folder and should contain csv-files which you want to convert.
The output directory is a folder where the resulting xes-files will be saved.

This way, you can automatically convert a collection of files at once.

User guide:
In mapping.properties, state which columns in your csv-files should be translated into the xes-file.

You can call the corresponding jar file in the following ways:
(1) Using the command-line (cd to the project directory):
java -jar "[install location]\CSVtoXESDir.jar" -i "[Input directory path]" -o "[Output directory path]"

(2) Call CsvToXesDirectory.bat. This file uses three parameters:
1. A local path to your java.exe file (inside the bin-directory of your local java installation)
2. The input directory (filled with csv files)
3. The output directory (where the xes files will be saved)
