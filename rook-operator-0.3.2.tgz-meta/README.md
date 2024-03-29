[![CircleCI](https://circleci.com/gh/giantswarm/rook-operator-app.svg?style=shield)](https://circleci.com/gh/giantswarm/rook-operator-app)

# rook-operator chart

Giant Swarm offers a rook-operator App which can be installed in workload clusters.
Here we define the rook-operator chart with its templates and default configuration.

**What is this app?**

This app deploys the [rook operator](https://github.com/rook/rook/) to Giant Swarm clusters.

**Why did we add it?**

Using Rook to provide Ceph storage abstracts storage provisioning away from the underlying
infrastructure and improves the end-user experience when interacting with storage.

**Who can use it?**

Anyone may use this app, however it is directly intended to be used in Giant Swarm on-premise
clusters.

## Installing

There are 3 ways to install this app onto a workload cluster.

1. [Using our web interface](https://docs.giantswarm.io/ui-api/web/app-platform/#installing-an-app)
2. [Using our API](https://docs.giantswarm.io/api/#operation/createClusterAppV5)
3. Directly creating the [App custom resource](https://docs.giantswarm.io/ui-api/management-api/crd/apps.application.giantswarm.io/) on the management cluster.

## Configuring

### values.yaml

**This is an example of a values file you could upload using our web interface.**

```
# values.yaml

```

### Sample App CR and ConfigMap for the management cluster

If you have access to the Kubernetes API on the management cluster, you could create
the App CR and ConfigMap directly.

Here is an example that would install the app to
workload cluster `abc12`:

```
# appCR.yaml

```

```
# user-values-configmap.yaml


```

See our [full reference page on how to configure applications](https://docs.giantswarm.io/app-platform/app-configuration/) for more details.

## Compatibility

This app has been tested to work with the following workload cluster release versions:

*

## Limitations

Some apps have restrictions on how they can be deployed.
Not following these limitations will most likely result in a broken deployment.

*

## Credit

* https://github.com/rook/rook/
