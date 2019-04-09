Cloud
=====

* Log transport - ingesting and sending logs wherever you want
    * Logstash
    * Fluentd
* Monitoring
    * [Prometheus](https://prometheus.io/)
* Messaging
    * [NATS](https://nats.io/)
        * Started by Derek Collison, who also started CloudFoundry
        * I prefer this to Kafka, mainly due to no JVM required
        * About twice as fast as Kafka
        * Much faster than RabbitMQ
    * Kafka
    * RabbitMQ
* API Gateway
    * [Kong](https://konghq.com/)
        * Sub-millisecond latency
        * 24k transactions/second (on a single node)
        * Built on Nginx, OpenResty, and Lua
* Log aggregation
    * Papertrail - aggregation, searching, alerting (inexpensive)
    * Splunk - aggregation, searching, alerting (expensive)
    * Scalyr - aggregation, searching, alerting (expensive)
    * [Loggly](https://www.loggly.com/) - aggregation, searching (inexpensive)
        * Might not have alerting
    * Flume - from Apache
        * Built with Java
        * Looks overly complex and difficult to configure
        * Stores in HDFS
        * Might not have good/simple alerting
    * Graylog2 - log aggregation, searching, alerting
        * Had a decent experience using this at CenturyLink, on WordPress team
        * Downside is storage is in Elastic and MongoDB
    * AWS Cloud Watch - worth investigating
    * ELK - I don't recommend (other than Logstash)
        * Too difficult to configure to get things back out
    * Scribe - from Facebook - no longer maintained
* Exception tracking
    * Sentry - open source or SaaS
    * ScoutApp - Rails and Elixir apps (pay)
* Coordination
    * Kubernetes
    * [Spinnaker](https://www.spinnaker.io) - continuous deployment
    * [Istio](https://istio.io) - service mesh to coordinate inter-service communication
* Dockerfile linting
    * [Hadolint](https://github.com/hadolint/hadolint)
