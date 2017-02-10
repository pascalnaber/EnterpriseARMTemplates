# Azure Service Bus with Topic

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResources%2FMicrosoft.ServiceBus(Topic)%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResources%2FMicrosoft.ServiceBus(Topic)%2Fazuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template deploys an Azure Service Bus with a Topic. The Topic can contain Subscriptions. You decide the name of the resources.

`Tags: Service Bus, Topic, Subscription`

## remarks

- If you want to deploy a service bus topic together with the service bus queue, 
  take a look at [this deployment sample](https://github.com/pascalnaber/EnterpriseARMTemplates/tree/master/DeploymentSamples/ServiceBusQueueAndTopicWithSubscriptions) how to do this. 

## supports

Besides the standard configuration

- Two authorization rules are added to the Topic. A Listen and a Send AuthorizationRule.


