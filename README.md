# Interactive Broker Java API
Interactive Broker Java API (IBAPI) is a copy of the original Interactive Brokers API to access TWS
platform.

## IB API Software
The original API can be accessed here (http://www.interactivebrokers.com/en/p.php?f=programInterface&p=a&ib_entity=llc)

## How to build IBAPI?
IBAPI is a Maven project. Please use the following commands to build:

* ```mvn compile``` - Compiles the project
* ```mvn package``` - Packages the project
* ```mvn install``` - Compiles, packages and installs the project in your local maven (m2) repository

## How to include IBAPI as a dependency in my project?

Below is the information about the project:
* ```com.ib.client``` - Group ID
* ```ibapi``` - Artifact ID
* ```1.0``` - Version #

### Play Framework

Append the following into your ```Build.scala```.
* ```"com.ib.client" % "ibapi" % "1.0"```

Add local Maven repository to your ```Build.scala```
```
resolvers += (
  "Local Maven Repository" at "file://"+Path.userHome.absolutePath+"/.m2/repository"
)
```

### Maven Project
```
<dependency>
    <groupId>com.ib.client</groupId>
    <artifactId>ibapi</artifactId>
    <version>1.0</version>
</dependency>
```