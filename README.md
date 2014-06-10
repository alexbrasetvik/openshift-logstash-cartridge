## OpenShift Logstash Cartridge

This is a simple cartridge for making Logstash easily available in your applications.


## Environment Variables

 * **`OPENSHIFT_LOGSTASH_ES_HOST`**: URL of the Elasticsearch cluster to log to. Required.
 * **`OPENSHIFT_LOGSTASH_ES_USERNAME`**: Username to connect as. Optional.
 * **`OPENSHIFT_LOGSTASH_ES_PASSWORD`**: Password to connect with. Optional.


=======
## Installation

First, configure the application with the appropriate environment variables. Then, add the cartridge to your application:

    $ rhc set-env --app my-app --namespace my-namespace --env "OPENSHIFT_LOGSTASH_ES_HOST=http://abc123-us-east-1.foundcluster.com:9200"
    $ rhc set-env --app my-app --namespace my-namespace --env "OPENSHIFT_LOGSTASH_ES_USERNAME=readwrite"
    $ rhc set-env --app my-app --namespace my-namespace --env "OPENSHIFT_LOGSTASH_ES_PASSWORD=secret"

## License

Released under the [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).