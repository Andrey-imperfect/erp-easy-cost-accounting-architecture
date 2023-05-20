# erp-easy-cost-accounting-architecture
The new architecture example for cost accounting which is 

(1) real-time 

(2) providing fully detailed results

(3) integrated into the operational ERP layer. 

(4) Besides, the calculation is complicated being adjusted by capacity of resources consumed (respectively to TD ABC cost accounting methodology), however is still transparent for end user and verifiable


***********************
The published code is written on "LsFusion" (a programming language specified for business applications compilating into Java).
***********************
How to install and run the LsFusion Programming Language:
1. Install JDK of 11.0.16 version. (Please, install exactly this version, not latest)
2. In IntelliJ IDEA, install LsFusion plug-in
3. Install Apache Tomcat of 9 version into the folder of JDK. (Plese, install exactly this version, not latest)
4. Download lsfusion-client-5.0.war
      Via this link: https://download.lsfusion.org/java
      
      Then, put this file into the folder of Tomcat -> Webapps [for example, C:\Program Files\Apache Software Foundation\Tomcat 9.0\webapps]

6. Download lsfusion-client-5.0.jar (via the same link)
8. Pull the project from GITHUB
9. In file erp-easy-cost-accounting-architecture.iml, change the row:

              <orderEntry type="library" name="C:\lsFusion\lsFusion 5\lsfusion-5.jar" level="application" />

            - please, after "name=" specify the address where "lsfusion-client-5.0.jar" is actually located
      
10. In file conf/setting.properties, specify address of your local infrastructure data (DB server) and also you may specify DB username / DB  password / DB name / LsFusion server port / LsFusion admin user password. 
Plese, pay attention that LsFusion platform will automatically create database after the first run.

12. To run the product:
      11.1. Run Apache Tomcat
      11.2. Run the project within IntelliJ IDEA
      11.3. Open file lsfusion-client-5.0.jar
