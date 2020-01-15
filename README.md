# outsystems-elastic-integration

This project contains the source code of Logstash and Kibana that allows with these tools of the [Elastic](elastic.co/) stack to be able:
1. Export OutSystems monitoring data from an OutSystems environment to Elasticsearch instance;
2. And be able to search, visualize and analyze that data on Kibana.

Note:
- For OutSystems monitoring data we consider:
    - Logs generated for the OutSystems Platform. Of the Platform itself and from the Applications that run on it.
    - Performance events captured by the Platform of itself and from 
        - Please be aware this type of monitoring data is only capture to OutSystems Web Traditional applications.


These Elastic accelerators were created because we see several OutSystems customers already having Elastic installations and wanting to leverage them to be able to observe, search and get deeper insights of the OutSystems monitoring data.


## Elastic accelerators
### Logstash
The Logstash code that allow to fetch OutSystems monitoring data from an OutSystems environment to Elasticsearch instance.

This is possible, for now, in one of two ways:
1. Getting data directly from OutSystems Logs tables through direct query (for now only usable for Microsoft SQL RDBMSs);
2. Getting data from the [OutSystems Performance API](https://success.outsystems.com/Documentation/11/Reference/OutSystems_APIs/PerformanceMonitoring_API).



### Kibana
The definitions on JSON that allow:
1. Defined an Elasticsearch mapping that allows to use more effectively the OutSystems Monitoring Data in Kibana and in particular allows to easily use the visualizations refered in 2;
2. The visualizations that allow to observe the data OutSystems monitoring data. In particular:
    1. Charts
    2. Dashboards


## Final notes
This code is maintained by the OutSystems Customer Success DevOps team to accelerate the ability of:
1. Easily observe of OutSystems monitoring data on Elastic with more advanced visualizations that the ones available natively on the OutSystems administration tools;
2. Easily search on OutSystems monitoring data (in particular doing free text search);
3. Do more advance monitoring that the ones available natively on the OutSystems administration tools. Like:
    1. Build an alerting system for an OutSystems environemnt or OutSystems Factory;
    2. Leverage Elastic analytics capabilities to have deeper insights of performance and behaviour of OutSystems Platform and applications;
    3. Etc.


In the future we intend to open the project repository to accept your contributions by pull requests.