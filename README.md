## objectscript-openapi-definition
This is a library for InterSystems ObjectScript.

The objectif of this library is to generate the ObjectScript Class from an OpenApi defintion.

## HowTo use it
To use class definition generator

Open a terminal and lunch this classmethod as this :

```objectscript
zw ##class(Grongier.OpenApi.Definition).Process("PetShop.spec")
```

Result is a new package in eg : PetShop.Definition with all the definition class ready to use.

## Installation with ZPM

```objectscript
zpm "install objectscript-openapi-definition"

```

## Installation with github

Clone/git pull the repo into any local directory

```sh
git clone https://github.com/grongierisc/objectscript-openapi-definition
```

Open the terminal in this directory and run:

```sh
docker-compose build
```

Run the IRIS container with your project:

```sh
docker-compose up -d
```

## How to Test it

Open IRIS terminal:

```sh
docker-compose exec iris iris session iris
USER>zn "IRISAPP"
IRISAPP>zw ##class(Grongier.OpenApi.Definition).Process("PetShop.spec")
```

## What's inside the repository

### Dockerfile

The dockerfile, create IRISAPP namespace, install code and the PetShop example.
