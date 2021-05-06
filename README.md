# Ranet Mondrian

Mondrian is an OLAP (Online Analytical Processing) server that enables business users to analyze large quantities of data in real-time. Mondrian is a Relation OLAP server (ROLAP). To store and manage the warehouse data, the relational OLAP uses relational or extended-relational DBMS.

Ranet Mondrian is a distribution of the Mondrian engine version, ready to use.

The main feature of this version is support of ADOMD.NET and Microsoft Excel clients.

This package is derived from xmondrian project: https://github.com/rpbouman/xmondrian


## Key Features

### Connect from Microsoft Excel to Mondrian Cube
Microsoft Excel is the most commonly used data analysis tool. It works great with SSAS OLAP cubes. 
Using Ranet Mondrian you shoot all oranicheniya Mondrian to work with Microsoft Excel.

### Advanced Cell Properties 
Support the FORE_COLOR and BACK_COLOR cell properties that store color information for the text and the background of a cell.

### High performance
High performance interactive analysis (Ad hoc) of large volumes of data.

### Free and open source
Ranet Mondrian is free to use under the Eclipse Public License (EPL).

## Getting Started

### Source code
The source code of the project is in the branch https://github.com/SergeiSemenkov/mondrian/tree/topsoft

### Deployment
1. Download *dist/ranetmondrian.war* file.
2. Copy *ranetmondrian.war* file to *webapps* directory of your java server (Apache Tomcat, Jetty, Tiny Java Web Server).
3. Open RanetMondrian homepage by navigating your browser to http://localhost:8080/ranetmondrian (8080 is port by default).

### Ranet Mondrian contains: 
- Official Mondrian documentation
- Ranet Mondrian Binaries
- Configuration files to deploy Ranet Mondrian to a servlet container (like Tomcat, Jetty, etc.)
- Sample databases
- XML/A commandline shell
- XML/A Analyzer and Visualizer

### Connect Microsoft Excel to Mondrian Cube:
- Open Microsoft Excel
- On **DATA** tab select **From Other Sources** item and then select **From Analysis Services**
- Enter http://localhost:8080/ranetmondrian/xmla as **Server name**

### Connect ADOMD.Net application to Mondrian Cube
To connect to mondrian from ADOMD.Net application you must use folowing connection string:

*Data Source=http://localhost:8080/ranetmondrian/xmla;*
