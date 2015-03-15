# README for Apache Fortress Demo End-to-End Security Example

## Last updated: March 15, 2015

## Prerequisites for target machine:
### 1. Debian or Redhat Liunx machine with OpenSSL installed.

### 2. Java 7 (or greater) sdk

### 3. Git

### 4. Apache Maven 3

### 5. Firefox Web Browser

### 6. Apache Fortress Ten Minute Guide:

    Follow the [directory-fortress-core.git] / README-TEN-MINUTE-GUIDE.txt
    https://git-wip-us.apache.org/repos/asf?p=directory-fortress-core.git.

    Complete these steps under 'Navigation Links':
####  a. Setup Apache Directory Server
####  b. Setup Apache Directory Studio
####  c. Build Apache Fortress Core
####  d. Build Apache Fortress Realm
####  e. Setup Apache Tomcat Web Server
####  f. Build Apache Fortress Web

## Instructions for downloading app and generating the install doc:

### 1. Download apache-fortress-demo package from github: https://github.com/shawnmckinney/apache-fortress-demo/archive/master.zip

### 2. Extract the zip archive to your local machine.

### 3. cd apache-fortress-demo-master

### 4. Set java and maven home env variables.

### 5. Run this command from the root package:
````
mvn javadoc:javadoc
````

note: if using java 8, add this param to the pom.xml:
````
<plugin>
    ...
    <artifactId>maven-javadoc-plugin</artifactId>
    <configuration>
        <additionalparam>-Xdoclint:none</additionalparam>
        ...
    </configuration>
</plugin>
````

### 6. Point your web browser to the following location:
file:///[apache-fortress-demo]//target/site/apidocs/overview-summary.html

(where [apache-fortress-demo] is location of this package)

### 7. Follow the steps under 'Demo Installation Instructions':
#### a. Heartbleed Bug
#### b. Managing PKI Keys
#### c. Set Hostname Entry
#### d. Apache Directory SSL
#### e. Apache Fortress Core SSL
#### d. Install MySQL
#### e. Apache Tomcat SSL
#### f. Apache Fortress Demo