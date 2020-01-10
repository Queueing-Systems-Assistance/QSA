# QSA Application  [![Website](https://img.shields.io/website-up-down-green-red/http/qsa.inf.unideb.hu.svg)](http://qsa.inf.unideb.hu/actuator/health)
QSA Application is a tool to visualize and calculate different queue properties. Main features:
- Calculate queue details
- Visualize queue properties

For those who want to help develop the application:
- [Git workflow](docs/git-workflow.md)
- [Useful links](docs/useful-links.md)

## Services

### qsa-application-config [![CLICK](https://img.shields.io/badge/-Click-blue)](https://github.com/Queueing-Systems-Assistance/qsa-application-config)
- system, it's properties and values configuration files
- tests for the configuration files

### qsa-application-backend [![CLICK](https://img.shields.io/badge/-Click-blue)](https://github.com/Queueing-Systems-Assistance/qsa-application-backend)
- contains all domain objects (POJOs)
- validates the domain objects
- here you can find the implementation of the math
- resolves systems and values, exception messages
- determines where is the request origin country

### qsa-application-frontend [![CLICK](https://img.shields.io/badge/-Click-blue)](https://github.com/Queueing-Systems-Assistance/qsa-application-frontend)
- user friendly website written in angular

## Contributors
- Szilágyi Zoltán
- Szászi Szabolcs
