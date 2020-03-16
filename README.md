# soa-readiness-checklist

Check your system for SOA readiness before start migration.

* communications
  * frontend - backend
  * backend - backend

* Events
  * event serealisation
    * TODO: take more examples from link - https://reasonablypolymorphic.com/blog/protos-are-wrong/index.html
    * binary
      * avro
      * protobuf
      * trift
    * humar readable 
      * xml
      * json
  * event types
  * Event ordering
  * Compatibility level and event versions
  * how to store event schemas
    * in source code
    * in separate library
    * in schema registry
  * event bus
    * if kafka
      * how to create a new topic locally, in production, in staging and in test env
      * topic convention
      * partition convention
      * consumer group
      * log compatction

* AuthN/AuthZ

* Data composition
  * How to make API composition
    * REST
      * API gateway
    * GraphQL
      * manual stitching
      * GQL gateway
  * How to make data composition
    * Sync
      * backend to backend communications
    * Async
      * event bus

* DevOps
  * Developers know how to provision a new service by self
  * Developers know how to setup CI/CD by self
  * Developers know how to deploy service to all env by self
  * Developers know how to setup logs/monitoring/alerting by self and where they can find all information about the service
  * Developers have clear understanding what they need to do from infrastructure perspective before start using a new service in production

* Testing
  * System has contract testing infrastructure
    * Developers can write contract testing without by self
  * System has e2e testing infrastructure

* Observability

## Links

* [Microservices Design Guide](https://medium.com/platform-engineer/microservices-design-guide-eca0b799a7e8)
* [When microservices fail...](https://docs.google.com/spreadsheets/d/1vjnjAII_8TZBv2XhFHra7kEQzQpOHSZpFIWDjynYYf0/edit#gid=0)
