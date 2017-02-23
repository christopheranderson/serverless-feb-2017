---
layout: slide
title: "Setup credentials"
classes:
data:
  transition: linear
---


{% highlight bash %}
azure login
azure account show # returns subscription and tentant
azure ad sp create -n <name> -p <password> # returns Service Principal Id & Object Id
azure role assignment create --objectId <objectIDFromCreateStep> -o Contributor
export azureSubId='<subscriptionId>'
export azureServicePrincipalTenantId='<tenantId>'
export azureServicePrincipalClientId='<servicePrincipalName>'
export azureServicePrincipalPassword='<password>'
{% endhighlight %}
