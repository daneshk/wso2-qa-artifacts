#How to handle XML body with processing instructions#

##Steps to verify the scenario##

1. Download WSO2 ESB from [1]
2. Extract it to a folder of your choice
3. Deploy the proxy service from the file system (Drop the CacheProxy.xml to $ESB_HOME/repository/deployment/server/synapse-configs/default/proxy-services)
4. Start the SampleAxis2 Server that is shipped with the product and make sure you have deployed the SimpleStockQuoteService as explained in [2]
4. Send a request to the Proxy service. The request payload is available in request.xml

`
E.g.:- curl -X POST -d @request.xml https://10.100.1.11:8243/services/PF -v -k
`
[1] - http://wso2.com/products/enterprise-service-bus/
[2] - https://docs.wso2.com/display/ESB481/Setting+Up+the+ESB+Samples#SettingUptheESBSamples-StartingtheAxis2server
