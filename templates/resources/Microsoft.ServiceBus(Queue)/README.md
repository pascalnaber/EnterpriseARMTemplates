# Azure Service Bus with Queue

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResources%2FMicrosoft.ServiceBus(Queue)%2Fazuredeploy.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fpascalnaber%2FEnterpriseARMTemplates%2Fmaster%2FResources%2FMicrosoft.ServiceBus(Queue)/azuredeploy.json" target="_blank">
    <img src="http://armviz.io/visualizebutton.png"/>
</a>

This template deploys an Azure Service Bus with a Queue. 

`Tags: Service Bus, Queue`

## remarks

- If you want to deploy a service bus topic together with the service bus queue, 
  take a look at [this deployment sample](https://github.com/pascalnaber/EnterpriseARMTemplates/tree/master/DeploymentSamples/ServiceBusQueueAndTopicWithSubscriptions) how to do this. 

## supports

Besides the standard configuration

- Two authorization rules are added to the Queue. A Listen and a Send AuthorizationRule.


