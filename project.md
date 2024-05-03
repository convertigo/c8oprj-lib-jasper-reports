
# ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/core/images/project_color_16x16.png?raw=true "Project") lib_JasperReports

This is the Jasper reports library for Convertigo Low Code Platform. Use this Library to generate PDF Reports  on data. The library is based on JasperSoft reporting library.

## Usage

You can provide a CSV files and a .jrxml report file to the library and call the GenerateReport Sequence. This will output a PDF report in the provided output path.

## Creating .jrxml files

These report description files can be authored using JaperSoft Studio (Download from [https://community.jaspersoft.com/download-jaspersoft/community-edition/] 

Your JRXML file must define a ROOT_PATH parameter to be used as prefix to any resource such as images used ion the report. See the data/Cherry_Landscape.jrxml sample

## Running the testcase

Run the testCase 'TestOK' to generate a sample PDF report. You will find the PDF report in the data/report.pdf file.

## File Paths

All file paths follows Convertigo file path resolution :
* .// is relative to the library project
* ./ is relative to the workspace
* Absolute path will not be modified

So if you want to resolve file paths before calling the library you can use 



```
 
	ResolvedPath = Engine.theApp.filePropertyManager.getFilepathFromProperty(pathToresolve, context.projectName)

```


	

<details><summary><span style="color:DarkGoldenRod"><i>Connectors</i></span></summary><blockquote><p>


## ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/connectors/images/sqlconnector_color_16x16.png?raw=true "SqlConnector") void

void connector, replace or don't use it

<details><summary><span style="color:DarkGoldenRod"><i>Transactions</i></span></summary><blockquote><p>


### ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/transactions/images/sqltransaction_color_16x16.png?raw=true "SqlTransaction") void

does nothing
</p></blockquote></details>
</p></blockquote></details>

<details><summary><span style="color:DarkGoldenRod"><i>Sequences</i></span></summary><blockquote><p>


<details><summary><b>AutoInit</b> : Initialize the lib on Linux systems and install needed dependencies</summary><blockquote><p>


## ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/sequences/images/genericsequence_color_16x16.png?raw=true "GenericSequence") AutoInit

Initialize the lib on Linux systems and install needed dependencies
</p></blockquote></details>

<details><summary><b>GenerateReport</b> : Generate a PDF report given a CSV file and a JRXML report file</summary><blockquote><p>


## ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/sequences/images/genericsequence_color_16x16.png?raw=true "GenericSequence") GenerateReport

Generate a PDF report given a CSV file and a JRXML report file

<span style="color:DarkGoldenRod">Variables</span>

<table>
<tr>
<th>
name
</th>
<th>
comment
</th>
</tr>
<tr>
<td>
<img src="https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/variables/images/variable_color_16x16.png?raw=true "  alt="RequestableVariable" >&nbsp;csvFileName
</td>
<td>
The CSV file name relative to the project's root
</td>
</tr>
<tr>
<td>
<img src="https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/variables/images/variable_color_16x16.png?raw=true "  alt="RequestableVariable" >&nbsp;jasperParams
</td>
<td>
An array of objects containing variable keys and values
</td>
</tr>
<tr>
<td>
<img src="https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/variables/images/variable_color_16x16.png?raw=true "  alt="RequestableVariable" >&nbsp;jrxmlFileName
</td>
<td>
The JRXML file relative to the project's root
</td>
</tr>
<tr>
<td>
<img src="https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/variables/images/variable_color_16x16.png?raw=true "  alt="RequestableVariable" >&nbsp;pdfFileName
</td>
<td>
The output PDF file relative to the projects's root
</td>
</tr>
</table>

</p></blockquote></details>

<details><summary><b>TestGenerateWithParams</b> : A test sequence to test passing parameters</summary><blockquote><p>


## ![](https://github.com/convertigo/convertigo/blob/develop/engine/src/com/twinsoft/convertigo/beans/sequences/images/genericsequence_color_16x16.png?raw=true "GenericSequence") TestGenerateWithParams

A test sequence to test passing parameters
</p></blockquote></details>
</p></blockquote></details>
