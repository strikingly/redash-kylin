# Introduction

At Strikingly we are using Apache Kylin as our BI solution to have insight about
multiple data sources. We are also using Redash, an excellent open source dashboard
service for drawing chart and generating report.

So we made this plugin to let redash connect to Kylin without configuring any JDBC connections.
After installed, you should be able to execute SQL query, test connections and list schemas upon
a Kylin data source.

## See also:

* Redash - https://redash.io/
* Apache Kylin - http://kylin.apache.org/

## Compatibility

* Redash - v3.0.0
* Apache Kylin - 2.x
 
## Installation:

1. Download redash v3.0.0 from https://github.com/getredash/redash/tree/v3.0.0
2. Copy `redash/query_runner/kylin.py` to the corresponding place in redash's folder
3. Enable `kylin.py` by adding `redash.query_runner.kylin` to `default_query_runners` defined
   in `redash/settings.py` or setting an environment variable
4. Deploy redash by building new docker images or choose your own way
5. Enjoy it!
 
## Usage:

1. Open redash in your browser
2. Add a new data source with admin account
3. Pick `kylin` as the data source type and fill in necessary fields
4. Start exploring data from Apache Kylin

# LICENSE

See [LICENSE](./LICENSE).
