## Steps to create complete folder from scratch:
```bash
mkdir hello-maven
cd hello-maven/
code .
touch pom.xml
mkdir -p src/main/java
cd src/main/java/
mkdir -p com/sivaacademy/devops
cd com/sivaacademy/devops/
touch utils.java
touch hellowworld.java
```
* Write the below content in utils.java and helloworld.java
```bash
// utils.java
package main.java.com.sivaacademy.devops;

public class utils {
    public String getName(){
        return "Devops with siva";
    }
}

// hellowworld.java
package main.java.com.sivaacademy.devops;

class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!!!");
    }
}
```
* Write the below content in pom.xml file
```xml
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    <groupId>com.sivaacademy.devops</groupId>
    <artifactId>hello-maven</artifactId>
    <version>1.0-SNAPSHOT</version>
</project>
```
* Execute the maven commands to compile/package/clean
```bash
# compile: goal will compile the source code and generates .class files in the target folder
mvn compile
# package will create the jar/war file as specified in pom.xml
mvn package
```
