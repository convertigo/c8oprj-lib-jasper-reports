


# lib_JasperReports

This is the Jasper reports library for Convertigo Low Code Platform. Use this Library to generate PDF Reports  on data. The library is based on JasperSoft reporting library.

## Usage

You can provide a CSV files and a .jrxml report file to the library and call the GenerateReport Sequence. This will output a PDF report in the provided output path.

## Creating .jrxml files

These report description files can be authored using JaperSoft Studio (Download from [https://community.jaspersoft.com/download-jaspersoft/community-edition/] 

Your JRXML file must define a ROOT_PATH parameter to be used as prefix to any resource such as images used ion the report. See the data/Cherry_Landscape.jrxml sample

## Running the testcase

Run the testCase 'TestOK' to generate a sample PDF report. You will find the PDF report in the data/report.pdf file.


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Sequences](#sequences)
    - [AutoInit](#autoinit)
    - [GenerateReport](#generatereport)
    - [TestGenerateWithParams](#testgeneratewithparams)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_JasperReports=https://github.com/convertigo/c8oprj-lib-jasper-reports.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_JasperReports=https://github.com/convertigo/c8oprj-lib-jasper-reports/archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_JasperReports__ project


## Sequences

### AutoInit

Initialize the lib on Linux systems and install needed dependencies

### GenerateReport

Generate a PDF report given a CSV file and a JRXML report file

**variables**

<table>
<tr>
<th>name</th><th>comment</th>
</tr>
<tr>
<td>csvFileName</td><td>The CSV file name relative to the project's root</td>
</tr>
<tr>
<td>jasperParams</td><td>An array of objects containing variable keys and values</td>
</tr>
<tr>
<td>jrxmlFileName</td><td>The JRXML file relative to the project's root</td>
</tr>
<tr>
<td>pdfFileName</td><td>The output PDF file relative to the projects's root</td>
</tr>
</table>

### TestGenerateWithParams

A test sequence to test passing parameters



