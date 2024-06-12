# Taller1ARSW

This is a introductory assigment made to understand and develop the "skeleton" of a program

## Getting Started
Link repositorio https://github.com/Parralol/Taller1ARSW
### Prerequisites
To be able to execute this programm you will need to execute

```
maven package
```

### Installing

First we need to execute the following command

```
mvn archetype:generate -DgroupId=edu.escuelaing.arsw.ASE.app -DartifactId=miprimera-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```
This will generate a folder with the following folder with it's branches

![image](https://github.com/Parralol/Lab01ARSW/assets/110953563/32a404db-56d9-4d62-b4e3-fa947c7ba97c)

With the following program

![image](https://github.com/Parralol/Lab01ARSW/assets/110953563/b9db96e4-7471-477a-909e-9474b95ad1e7)

and it's corresponding tests

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/dc6ab22b-53d0-4477-ab56-a4dce3e407d1)




## Configuration
once everything is in place we proceed to execute 
```
mvn package
```
and when we get  BUILD SUCCESS (like in the following image)

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/03d9522f-4fb6-4107-8f8a-9c884a716453)

we will be sure that it is working

To be run the following program you need to be in the program directory, once inside enter

```
mvn site
```
to generate the folder in which the documentation will be stored, now, we need to change the pom, we will change it like this:

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/d05d4ee2-3f46-4f27-9d29-62895ce4701f)

this is just to be able to generate javadoc, once entered we will type all of the following commands:

```
mvn javadoc:javadoc
```
```
mvn javadoc:jar
```
```
mvn javadoc:aggregate
```
```
mvn javadoc:aggregate-jar
```
```
mvn javadoc:test-javadoc
```
```
mvn javadoc:test-jar
```
```
mvn javadoc:test-aggregate
```
```
mvn javadoc:test-aggregate-jar
```
(in order)

this will create the following files:

![image](https://github.com/Parralol/Taller1ARSW/assets/110953563/47decd48-675b-494f-b519-253e929a53f0)


## Running the tests

to run the tests you need to execute 

```
mvn test
```

## Deployment

Once all the steps above have been completed, we will package the proyect with 

```
mvn package
```

then, we execute

```
java -cp target/miprimera-app-1.0-SNAPSHOT.jar edu.escuelaing.arsw.ASE.app.App
```
## Build with

* Maven
* Java

## Authors

* Santiago Parra
