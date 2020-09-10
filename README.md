# Partido Server
<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
[![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
<!-- ALL-CONTRIBUTORS-BADGE:END -->
![CI](https://github.com/jens-wagner/partido-server/workflows/CI/badge.svg)

This is the backend server application of the Partido platform written in Java with the Spring Framework.

Partido itself is a platform independent App for sharing group expenses.

## How to run the server

In the project root folder, run:

```
mvn spring-boot:run
```

or just press the IDE's run button.

The server will listen on Port 8080 per default (defined in `./src/main/resources/application.properties`).

## Database

The server needs an already existing PostgreSQL database.

The defaults defined in `./src/main/resources/application.properties` are:

```
## Spring DATASOURCE (DataSourceAutoConfiguration & DataSourceProperties)
spring.datasource.url=jdbc:postgresql://localhost:5432/partido-server
spring.datasource.username=postgres
spring.datasource.password=postgres
```

You can override these properties with custom start parameters.

## Mail sending on local machine

Per default, the server tries to send emails to localhost on Port 25 without any credentials.
If you don't have a (fake) Mailserver installed, the console will output some specific errors, you can ignore. If you want to get those emails, you can use a tool like FakeSMTP: http://nilhcem.com/FakeSMTP/

## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://www.fosforito.de"><img src="https://avatars3.githubusercontent.com/u/5000255?v=4" width="100px;" alt=""/><br /><sub><b>Jens Wagner</b></sub></a><br /><a href="https://github.com/jenslw/partido-server/commits?author=jenslw" title="Code">💻</a> <a href="#translation-jenslw" title="Translation">🌍</a> <a href="#infra-jenslw" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#maintenance-jenslw" title="Maintenance">🚧</a> <a href="https://github.com/jenslw/partido-server/commits?author=jenslw" title="Tests">⚠️</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!
