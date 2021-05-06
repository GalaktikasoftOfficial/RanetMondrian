# RanetMondrian
Ranet Mondrian is a distribution of the Mondrian (R)OLAP engine version.

The main feature of this version is support of ADOMD.NET and Excel clients.
This package is derived from xmondrian project: https://github.com/rpbouman/xmondrian

## Source code
The source code of the project is in the branch https://github.com/SergeiSemenkov/mondrian/tree/topsoft

## Deployment
1. Download *dist/ranetmondrian.war* file.
2. Copy *ranetmondrian.war* file to *webapps* directory of your java server (Apache Tomcat, Jetty, Tiny Java Web Server).
3. Open RanetMondrian homepage by navigating your browser to http://localhost:8080/ranetmondrian (8080 is port by default).

## RanetMondrian contains: 
- Official Mondrian documentation
- Ranet Mondrian Binaries
- Configuration files to deploy Ranet Mondrian to a servlet container (like Tomcat, Jetty, etc.)
- Sample databases
- XML/A commandline shell
- XML/A Analyzer and Visualizer

## Connect Microsoft Excel to Mondrian Cube:
- Open Excel
- On **DATA** tab select **From Other Sources** item and then select **From Analysis Services**
- Enter http://localhost:8080/ranetmondrian/xmla as **Server name**

## Connect ADOMD.Net application to Mondrian Cube
To connect to mondrian from ADOMD.Net application you must use folowing connection string:

*Data Source=http://localhost:8080/ranetmondrian/xmla;*

