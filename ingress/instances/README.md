# Ingress

This is the section where loadbalancers and domain association are defined.

Here there are two ingress defined namely *demoingress* and *tools*

## demoingress

* By default it creates a default domain of demoingress-<clusterid>.<customer-name>.console.facets.cloud. For example if you have created a cluster with id cluster1 and your control plane url is `company.console.facets.cloud` you can access your ingress at `demoingress-cluster1.company.console.facets.cloud`
* You can further associate custom domains to this per cluster from UI, for example in your qa cluster you can map `qa.company.com` to this ingress and then u can access it via that name
