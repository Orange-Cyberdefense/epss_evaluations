## Getting started

To use this tool you'll require to open the "index.html" file using a browser. Two files must be supplied namely the "Vulns CSV file" and the "Exploited Vulns CSV file". The first Comma Separated Value (CSV) file is intended to represent a superset of vulnerabilities that is present in a given environment. The second CSV file is a subset of vulnerabilities present in the first file and represents exploited vulnerabilities. Note that CVEs in the second CSV file must be present in the first Vuln file.

The CSV files must be formatted in a specific way. The first line of both text files should be the headers and must contain a "cve" column and an "epss" column. A comma (,) must be used to separate the columns. Each record should be on a new line. Microsoft Excel save CSV files with semicolon (;) by default. Excel must be explicitly configured to save CSV files with commas (,) instead of semicolon (;).

The "Upload File" button must be pressed to process the specified files. A record count or total will be shown below the file path once calculated successfully.

The "Chart" and "Calculate Strategy" sections will produce meaningful output after the two CSV files were processed successfully. The buttons lablled "Plot", "Calc", and "Download CSV" must be pressed to generate output.

*NOTE:* The "Plot" feature may take a significant amount of time as the JavaScript to generate the line chart has not been optimised. The amount of time taken to draw the chart may depend on the number of records supplied and the platform hosting the browser. Expect this to take between 10 to 30 seconds.

The "Download CSV" button in the "Calculate Strategy" section will produce a CSV file that contains the CVEs with each respective EPSS for the supplied EPSS value.

## Authors and acknowledgment
This project uses the following JavaScript libraries:
* JQuery
* Bootstrap
* MathJS
* PapaParse for CSV processing (https://github.com/mholt/PapaParse)
* Plotly for Charts (https://plot.ly)

## License
This project is licensed in terms of MIT License (MIT).

## Disclaimer
This project is provided as-is and no guarantee is provided or implied. Please verify output independently and if you wish to incorporate some or all of the features then verify completely.

## Project status
This project is considered a work in progress and may be updated as the need arise or as any party sees fit.
