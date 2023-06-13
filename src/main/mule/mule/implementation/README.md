Mule API starter project template

This Template API is a mule api project template that you can use as a starting point for development of your own implementation with exchangeAPI to get connector version difference.

First we need to get token to connect to anypoint exchange. Token is stored for 1hr in cache.

This API will check connector version present in pom file and then it will call exchange api for that particular assest to get the latest version details present in exchange API.
If there is any difference in version then it will return the output for those connector only..

sample response::

[
    {
        "connectorName": "mule-http-connector",
        "connectorGroupName": "org.mule.connectors",
        "currentVersionInApi": "1.7.1",
        "latestVersionInExchange": "1.7.3"
    },
    {
        "connectorName": "mule-sockets-connector",
        "connectorGroupName": "org.mule.connectors",
        "currentVersionInApi": "1.2.2",
        "latestVersionInExchange": "1.2.3"
    },
    {
        "connectorName": "mule-objectstore-connector",
        "connectorGroupName": "org.mule.connectors",
        "currentVersionInApi": "1.2.0",
        "latestVersionInExchange": "1.2.1"
    }
]