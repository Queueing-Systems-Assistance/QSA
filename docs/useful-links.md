## Useful Links

### [Elastic Search](http://qsa.inf.unideb.hu/kibana)

- Elastic Search is responsible for catching and storing the logs from QSA Backend
- QSA Backend is logging throw a HTTP request to the Logstash

### [Graphite](http://qsa.inf.unideb.hu/graphite)

- Carbon is responsible for receiving metrics, caching and persisting them to disk.

### [Grafana](http://qsa.inf.unidebhu/grafana)

- Data visualization & Monitoring with support for Graphite

### [Portainer](http://qsa.inf.unideb.hu/portainer)

- Portainer is a powerful, open-source management toolset that allows you to easily build, manage and maintain Docker environments

### [Sonar Cloud](https://sonarcloud.io/dashboard?id=ZoltanSzilagyiCse_QSA)

- SonarCloud automatically analyzes QSA source code on master branch
- It is useful for inspect the quality of source code and detect bugs, vulnerabilities and code smells

### [Travis CI](https://travis-ci.com/ZoltanSzilagyiCse/QSA)

- Travis CI is a hosted, distributed continuous integration service used to build and test QSA
- Automatically detects when a commit has been made and pushed to QSA. Each time this happens, it will try to build the project and run tests.