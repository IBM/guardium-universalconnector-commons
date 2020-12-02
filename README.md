# Guardium Universal-Connector Commons
This project contains helper classes & utilities for creating a Guardium Record – a required object while developing a plugin for [Guardium universal connector][KC-UC-main], a feature within IBM Security Guardium. 

## How to use it
1. Clone this project
2. Build the JARs by running `./gradlew.unix assemble` or `./gradlew.bat assemble` on Windows. 
    This will create 3 JAR files containing the compiled code, javaDocs, and sources.
3. Clone or download [logstash-filter-mongodb-guardium][] example project. 
4. Within your plugin project, create _gradle.properties_ 
    and add a reference to the folder with the built JAR files. For example: 

    ```GUARDIUM_UNIVERSALCONNECTOR_COMMONS_PATH=../guardium-universalconnector-commons/build/libs```
    
    The GUARDIUM_UNIVERSALCONNECTOR_COMMONS_PATH variable is used in _build.gradle_, when compiling and building the code in your plugin project.

5. Link the javadoc and sources JAR files from within your preferred IDE, to assist you in your development. 

## Contribute
See [CONTRIBUTING.md] for ways to raise issues, fix them, discuss enhancements, and just sending us feedback. 

<!-- links -->
[KC-UC-main]: https://www.ibm.com/support/knowledgecenter/SSMPHH_11.3.0/com.ibm.guardium.doc.stap/guc/g_universal_connector.html

[logstash-filter-mongodb-guardium]: https://github.com/IBM/logstash-filter-mongodb-guardium

[CONTRIBUTING.md]: ./CONTRIBUTING.md
