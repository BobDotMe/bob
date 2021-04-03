# Documentation
# BoB!  Quickstart
This guide will walk you through the basic setup of BoB! enable the backend services.
## Minimum Version
Kubernetes **v1.15** or higher is supported by BoB!.
Helm version **3.x** or higher is supported by BoB!.

## TL;DR
If you're feeling lucky, a simple BoB! cluster can be created with the following `helm 3` command.  No `values.yaml` is necessary. For the more detailed install, skip to the next section to [deploy the BoB! cluster](#deploy-the-bob-cluster).
    
***console***
```
#Set the version to a production semantic version
helm3 report add 262life https://262life.github.io/bob    
kubectl create namespace bob
helm3 update --install bob 262life/bob --version 0.9.13
```

After the cluster is running, you must now install the BoB! plugins.  You WILL require administrator proviledges on your workstation or server to do so.  This is NOT intended to be installed on the K8s hosts.

***console***
```
#Set the version to a production semantic version
export vers="v0.9.13"; curl --location --silent -o - https://github.com/262life/bob/releases/download/${vers}/installer.sh | bash -s -- ${vers}
```
## kubectl plugin
Details on the plugin can be found [here](commands.md).
## Deploy the BoB! Cluster


The first step is to deploy the BoB! cluster. Check that you are using ...
    
***console***
```
helm3 install bob bob/bob --version 0.8-var7-rc.5 --set  "image.pullPolicy=Always"
```
## Upgrading

To upgrade the BoB! cluster, simply upgrade the helm chart.

***console***
```
helm3 upgrade  bob bob/bob --version v0.8.7-rc.5 [--devel]
```

## Teardown

To teardown the BoB! cluster, simply uninstall the helm chart.

***console***
```
#helm3 delete bob 
```
