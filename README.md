Convo
-----

Convo is a specification-based voice and text conversation library.

A Convo application consists of the following components:
1. A mandatory [Dialogflow](https://dialogflow.com/) agent which provides various devices and services integration
2. An optional [Google Cloud Functions](https://cloud.google.com/functions/) middleware which provides back-end implementation

Architectures
-------------

There are three types of Convo application architectures:

1. Static Facts

Convo Static Facts application consists of only a Dialogflow agent where its knowledge comprises of static facts within the agent itself. 

![Convo Static Facts architecture diagram](https://github.com/cliffano/convo/raw/master/docs/architecture-static-facts.png "Convo Static Facts architecture diagram")

Have a look at [Convo Thomas](http://github.com/cliffano/convo-thomas) for an example of Convo Static Facts application.

2. Freestyle Back-End

Convo Freestyle Back-End application consists of a Dialogflow agent and a Freestyle CloudFunctions middleware where its knowledge is sourced from the business logic implemented within the middleware.

![Convo Freestyle Back-End architecture diagram](https://github.com/cliffano/convo/raw/master/docs/architecture-freestyle-backend.png "Convo Freestyle Back-End architecture diagram")

Have a look at [Convo Hacker News](http://github.com/cliffano/convo-hacker-news) for an example of Convo Freestyle Back-End application, along with [Convo Hacker News Helper](http://github.com/cliffano/convo-hacker-news-helper) which provides the freestyle back-end implementation.

3. OpenAPI Back-End

Convo Freestyle Back-End application consists of a Dialogflow agent and an OpenAPI CloudFunctions middleware where its knowledge is sourced from an external [Open API](https://www.openapis.org/) service.

![Convo OpenAPI Back-End architecture diagram](https://github.com/cliffano/convo/raw/master/docs/architecture-openapi-backend.png "Convo OpenAPI Back-End architecture diagram")

Have a look at [Convo Jenkins](http://github.com/cliffano/convo-jenkins) for an example of Convo OpenAPI Back-End application, along with [Convo Jenkins Helper](http://github.com/cliffano/convo-jenkins-helper) which provides the OpenAPI and Jenkins utilities back-end implementation.

Configuration
-------------

Usage
-----

1. Create the configuration files for the corresponding Convo application architecture

Colophon
--------

Related Projects:

* [Convo Generator](http://github.com/cliffano/convo-generator) - Convo agent and middleware generator
* [convo-node](http://github.com/cliffano/convo-node) - node.js utility module for Convo voice library
* [Convo Thomas](http://github.com/cliffano/convo-thomas) - Convo agent for Thomas the Tank Engine Facts
* [Convo Hacker News](http://github.com/cliffano/convo-hacker-news) - Convo agent and middleware for Hacker News
* [Convo Hacker News Helper](http://github.com/cliffano/convo-hacker-news-helper) - Helper node.js module for Convo Hacker News
* [Convo Jenkins](http://github.com/cliffano/convo-jenkins) - Convo agent and middleware for Jenkins
* [Convo Jenkins Helper](http://github.com/cliffano/convo-jenkins-helper) - Helper node.js module for Convo Jenkins
