JSON Schema Generator for Kubernetes v1.6.2 API Objects
=========================================================

Uses Go reflection to generate a JSON schema that describes one or more 
API resources in Kubernetes.

Pre-requisites
-------------

Install [go](https://golang.org/doc/install)   
Install [godep](https://github.com/GoogleCloudPlatform/kubernetes/blob/master/docs/devel/development.md#godep-and-dependency-management)   

Building
--------
To build, clone repo and run:  

```
glide install --strip-vendor --strip-vcs
go build ./cmd/generate
generate > ./kubernetes-model/src\main/resources/schema/kube-schema.json
mvn clean install
```