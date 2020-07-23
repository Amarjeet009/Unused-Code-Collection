# Unused-Code-Collection
How to install MAVEN in Windows 10 using CMD
1. JDK and JAVA_HOME
Make sure JDK is installed, and JAVA_HOME environment variable is configured.

2. Download Apache Maven
2.1 Visit Maven official website, download the Maven zip file, for example : apache-maven-3.6.0-bin.zip.
http://maven.apache.org/download.cgi
2.2 Unzip it to a folder. In this article, we are using c:\opt\apache-maven-3.6.0
3. Add MAVEN_HOME system variable
Add a MAVEN_HOME system variables, and point it to the Maven folder.

3 Press Windows key, type adva and clicks on the View advanced system settings
--> In “Environment variables” dialog, System variables, Clicks on the New... 
button and add a MAVEN_HOME variable and point it to c:\opt\apache-maven-3.6.0

4. Add %MAVEN_HOME%\bin To PATH
In system variables, find PATH, clicks on the Edit... button. In “Edit environment variable” dialog, clicks on the New button and add this %MAVEN_HOME%\bin
5. Verification
Done, start a new command prompt, type
mvn –version


How to Create MAVEN in Windows 10 using CMD

mvn archetype:generate
	-DgroupId={project-packaging}
	-DartifactId={project-name}
	-DarchetypeArtifactId={maven-template}
	-DinteractiveMode=false
	
mvn archetype:generate -DgroupId=com.amar.hashing -DartifactId=hashing-project -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false


Add SQL Server Dependency 
Download Dependency and save in your local:

mvn install:install-file -Dfile=sqljdbc4.jar -DgroupId=com.microsoft.sqlserver -DartifactId=sqljdbc4 -Dversion=4.0 -Dpackaging=jar



mvn install:install-file -Dfile=C:\sqljdbc4.jar -DgroupId=com.microsoft.sqlserver -DartifactId=sqljdbc4 -Dversion=4.0.2206.100 -Dpackaging=jar


mvn install:install-file -Dfile=E:\sts-project-space-2020\sqljdbc4-4.0.jar -DgroupId=com.microsoft.sqlserver -DartifactId=sqljdbc4 -Dversion=4.0 -Dpackaging=jar

==================================
-startup
plugins/org.eclipse.equinox.launcher_1.5.700.v20200207-2156.jar
-vm
C:/Program Files/Java/jdk1.8.0_144/bin/javaw.exe
-Dosgi.requiredJavaVersion=1.8
-Xms256m
-Xmx1024m
-XX:+UseG1GC
-XX:+UseStringDeduplication
--add-modules=ALL-SYSTEM
--launcher.library
plugins/org.eclipse.equinox.launcher.win32.win32.x86_64_1.1.1200.v20200508-1552
-product
org.springframework.boot.ide.branding.sts4
--launcher.defaultAction
openFile
-vmargs
-Dosgi.requiredJavaVersion=1.8
-Xms256m
-Xmx1024m
-XX:+UseG1GC
-XX:+UseStringDeduplication
--add-modules=ALL-SYSTEM




