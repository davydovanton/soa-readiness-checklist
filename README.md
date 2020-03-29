# soa-readiness-checklist

Check your system for SOA readiness before start migration.

## Checklist

SOON


## Raw topics

* communications
  * frontend - backend
    * Types
      * json API
      * REST json
      * GraphQL
    * Guidelines for developers

  * backend - backend
    * Types
      * json API
      * REST json
      * GraphQL
      * AvroRPC
      * gRPC
      * Thrift RPC
    * Guidelines for developers

* Events
  * event serealisation
    * TODO: take more examples from link - https://reasonablypolymorphic.com/blog/protos-are-wrong/index.html
    * humar readable
      * xml
      * json
    * binary
      * avro
      * protobuf
      * trift
    * Links
      * http://dataintensive.net

  * event types
    * Business event
      * High-level, intention-revealing business events

    * Data-change event
      * Low-level, technical event for describing changes

    * Links
      * "Format & Semantics" section from https://medium.com/@sderosiaux/cqrs-what-why-how-945543482313

  * Event ordering
    * by event bus
    * by service logic

  * Compatibility level and event versions
    * backward and forward compatibility
    * Different versions for event data and event schema
    * Links
      * http://dataintensive.net

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
    * if rebbitmq
      * how to create a queue
    * if google pub/sub
      * how to create a queue

* AuthN/AuthZ

* Data composition
  * How to make API composition
    * REST
      * API gateway
        * self written
        * open source
    * GraphQL
      * manual stitching
      * GQL gateway

  * How to make data composition
    * Sync
      * backend to backend communications
    * Async
      * event bus

  * Data synchronization
    * How to get data which needful for business logic?
      * sync way
        * Backend to backend communications
      * async way
        * event bus
        * CQRS
        * data streaming

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
  * Logs
    * Developers know how to store logs
    * everyone know how and where to read logs
  * Monitoring
    * Business metrics
    * ARP metrics
    * System metrics
    * Tracing

* Inventory aka list of all services in the system
  * We need a place where we can see all our services and dependencies between them

* local development
  * developers can get same env as a production env

* ETL and analytics

* Documentation
  * Do you have a process around Architecture Decision Records?
  * Do you have domain documentation which can be useful for developers and other ppl from the team?
  * Do you have a documentation for the each service?
    * API
    * architecture of the service
    * how to install service locally
  * List of allowed technologies/practices
  * Checks
    * deployment checklist
    * moving to production checklist


## Links

* [Microservices Design Guide](https://medium.com/platform-engineer/microservices-design-guide-eca0b799a7e8)
* [When microservices fail...](https://docs.google.com/spreadsheets/d/1vjnjAII_8TZBv2XhFHra7kEQzQpOHSZpFIWDjynYYf0/edit#gid=0)
