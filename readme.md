


# lib_JasperReports

This is the Jasper reports library for Convertigo Low Code Platform. Use this Library to generate PDF Reports  on data. The library is based on JasperSoft reporting library.

## Usage

You can provide a CSV files and a .jrxml report file to the library and call the GenerateReport Sequence. This will output a PDF report in the provided outpout path.

## Creating .jrxml files

These report description files can be authored using JaperSoft Studio (Download from [https://community.jaspersoft.com/download-jaspersoft/community-edition/] 

Your JRXML file must define a ROOT_PATH parameter to be used as prefix to any resource such as images used ion the report. See the data/Cherry_Landscape.jrxml sample

## Running the testcase

Run the testCase 'TestOK' to generate a sample PDF report. You will find the PDF report in the data/report.pdf file.


For more technical informations : [documentation](./project.md)

- [Installation](#installation)
- [Mobile Library](#mobile-library)


## Installation

1. In your Convertigo Studio click on ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/icons/studio/project_import.gif?raw=true "Import a project in treeview") to import a project in the treeview
2. In the import wizard

   ![](https://github.com/convertigo/convertigo/blob/develop/eclipse-plugin-studio/tomcat/webapps/convertigo/templates/ftl/project_import_wzd.png?raw=true "Import Project")
   
   paste the text below into the `Project remote URL` field:
   <table>
     <tr><td>Usage</td><td>Click the copy button at the end of the line</td></tr>
     <tr><td>To contribute</td><td>

     ```
     lib_JasperReports=C:/Users/opic_000/runtime-EclipseApplication/lib_JasperReports/.git:branch=master
     ```
     </td></tr>
     <tr><td>To simply use</td><td>

     ```
     lib_JasperReports=C:/Users/opic_000/runtime-EclipseApplication/lib_JasperReports//archive/master.zip
     ```
     </td></tr>
    </table>
3. Click the `Finish` button. This will automatically import the __lib_JasperReports__ project


## Mobile Library

Describes the mobile application global properties



