<img align="left" width="100" height="100" style="margin: 25px 25px 5px 5px" src="images/discipl.svg">

## D I S C I P L
This repository contains common resources and documentation
shared by all projects in the Discipl Software Stack.

![](images/discipl-infographic.png)

## Discipl information

- [Homepage](https://discipl.org)
- [Principles](https://discipl.org/home/technology/)
- [Collaboration](https://discipl.org/home/collaboration/)
- [Dynamic matching system](https://discipl.org/home/collaboration/dms/)
- [Roadmap](https://discipl.org/home/roadmap/)
- [Slack](https://discipl.slack.com) ([No access?](https://join.slack.com/t/discipl/shared_invite/enQtOTYwNzUxNDk0NzA3LWRhYTNjMThhM2JlNTRjYjdlZjA2Mjc4OGY1NTU3ZjY2YTUxNjYzMDU5OGI3NWQ3Mzc3ZjQ1MjU1ODJkMmU5M2U))

## Discipl Components

### Discipl Core [![Build Status](https://travis-ci.org/discipl/core.svg?branch=master)](https://travis-ci.org/discipl/core)

[Discipl Core](https://github.com/discipl/core) provides an interface to connect to different platforms that manage identities and claims.

Sample usage:

- [Creating an identity](https://github.com/discipl/core/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L24)
- [Storing and retrieving a claim](https://github.com/discipl/core/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L39)
- [Verifying an attestation](https://github.com/discipl/core/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L64)
- [Listening for claims being published by an identity](https://github.com/discipl/core/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L118)
- [Managing access](https://github.com/discipl/core/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L396)

### Discipl Core Ephemeral Connector [![Build Status](https://travis-ci.org/discipl/discipl-core-ephemeral.svg?branch=master)](https://travis-ci.org/discipl/discipl-core-ephemeral)

The [Ephemeral Connector](https://github.com/discipl/discipl-core-ephemeral) provides temporary storage of identities and claims. 
This can be done using a local memory storage or a remote storage, and elliptic curve cryptography or RSA (based on x509 certificates).

- [Instantiating and configuring](https://github.com/discipl/discipl-core-ephemeral/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L122)
- [Importing an identity](https://github.com/discipl/discipl-core-ephemeral/blob/e700e783e21b1f960f691539d89f4c34fb1074ba/test/index.spec.js#L44)

### Discipl Core Base Connector [![Build Status](https://travis-ci.org/discipl/discipl-core-baseconnector.svg?branch=master)](https://travis-ci.org/discipl/discipl-core-baseconnector)

The [Core Base Connector](https://github.com/discipl/discipl-core-baseconnector) can be used to implement a connector to your platform of choice.

- [Mock connector showing the needed methods](https://github.com/discipl/discipl-core-baseconnector/blob/3eed4482bd57ceb7233cd396ca5a52156d5ad394/test/base-connector.spec.js#L8)
- [Usage example (Ephemeral)](https://github.com/discipl/discipl-core-ephemeral/blob/3eed4482bd57ceb7233cd396ca5a52156d5ad394/src/EphemeralConnector.js#L13)

### Discipl Abundance Service [![Build Status](https://travis-ci.org/discipl/discipl-abundance-service.svg?branch=master)](https://travis-ci.org/discipl/discipl-abundance-service)

The [Abundance Service](https://github.com/discipl/discipl-abundance-service) helps implementation of software systems that express needs and fulfill them.

- [Example scenario](https://github.com/discipl/discipl-abundance-service/blob/1ab9e02bec7367477b56efc2cca4c07e24240bd6/test/index.spec.js#L38)
- [Attending to needs in Waardepapieren Project](https://github.com/discipl/waardepapieren/blob/4532cf36c7f560b16c71a65b9f9b5e253d0d5753/waardepapieren-service/src/waardepapieren-service.js#L42)
- [Expressing needs in Waardepapieren Project](https://github.com/discipl/waardepapieren/blob/4532cf36c7f560b16c71a65b9f9b5e253d0d5753/clerk-frontend/src/need-wizard/ConfirmStep.js#L24)

### Discipl Paper Wallet [![Build Status](https://travis-ci.org/discipl/discipl-paper-wallet.svg?branch=master)](https://travis-ci.org/discipl/discipl-abundance-service)

The [Paper Wallet](https://github.com/discipl/discipl-paper-wallet) helps convert claims to a qr-format for presentation.

- [Example scenario](https://github.com/discipl/discipl-paper-wallet/blob/96e4289438e4ef564e3a01803cae6d2dd9b655ac/test/index.spec.js#L19)
- [Example usage in Waardepapieren Project](https://github.com/discipl/waardepapieren/blob/4532cf36c7f560b16c71a65b9f9b5e253d0d5753/clerk-frontend/src/need-wizard/DeliveryStep.js#L33)


## Discipl Law Reg [![Build Status](https://travis-ci.org/discipl/discipl-law-reg.svg?branch=master)](https://travis-ci.org/discipl/discipl-law-reg)

The [Law Reg(ulation)](https://github.com/discipl/discipl-law-reg) library provides validation and execution options for FLINT models. 
FLINT is a (formal) language to interpret laws and regulation.

- [Theoretical background and example](http://ceur-ws.org/Vol-2471/paper6.pdf)
- [Example model in JSON form](https://github.com/discipl/discipl-law-reg/blob/2d8aeb66f126dc7a897084a8957300d9c414405f/test/Vreemdelingenwet.flint.json)
- [Usage in demo interface](https://github.com/discipl/ComplianceByDesign/blob/69609d428725a65661ac633265607b50195860c9/compliance-by-design-demo/src/components/ActorView.js#L81)


## Discipl Projects

### Waardepapieren [![Build Status](https://travis-ci.org/discipl/waardepapieren.svg?branch=master)](https://travis-ci.org/discipl/waardepapieren)

The [Waardepapieren](https://github.com/discipl/waardepapieren) project showcases how the abundance service and core Discipl components
can be used by a municipality to provide attestations that are backwards compatible with current processes.

### Compliance by Design [![Build Status](https://travis-ci.org/discipl/ComplianceByDesign.svg?branch=master)](https://travis-ci.org/discipl/ComplianceByDesign)

[Compliance by Design](https://github.com/discipl/ComplianceByDesign) showcases how FLINT models produced using the Calculemus method can be explored.
A way to create these models is using Visual Studio Code with the [FLINT editor plugin](https://github.com/discipl/flinteditor-vscode)

### Tools and Techniques the projects are using

- Node.js
  ```
  Node.js is used as the run-time environment to execute this program written in JavaScript. It also comes with a built-in support for package management using NPM. Discipl publishes her libraries in NPM.
  ```
- ES6 JavaScript
  ```
  ES6 stands for EcmaScript 6 and is a version of Javascript
  ```
- Travis CI
  ```
  Travis CI is a hosted continuous integration service used to build and test software projects hosted at GitHub.
  ```
- Babel
  ```
  Babel is used to transpile the ES6 to get compatible JavaScript
  ```
- Mocha - Chai - SinonJS
  ```
  Sinon allows the use of spies, stubs and mocks within the tests.
  Chai will make the coding of the test feel like writing english.
  To use Chai and Sinon, Mocha is needed as the test framework running on Node.JS
  ```
- Istanbul code coverage
  ```
  All-javascript instrumentation library that tracks statement, branch, and function coverage and reverse-engineers line coverage with 100% fidelity.
  ```
- Standard JS lint
  ```
  Automatically formats the code and catches style issues and programmer errors early.
  ```
- LogLevel
  ```
  Minimal lightweight simple logging for JavaScript. loglevel replaces console.log() and friends with level-based logging and filtering, with none of console's downsides.
  ```
