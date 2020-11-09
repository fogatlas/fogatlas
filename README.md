# FogAtlas

## What is FogAtlas

FogAtlas is a platform for intelligently placing microservice-based applications
on the cloud-to-edge continuum.

It is based on Kubernetes and indeed it is an extension of Kubernetes (thanks to the k8s CRD
mechanism) for fog computing environments.

## FogAltas components

FogAtlas is composed by:
1. some [Custom Resource Definitions](https://github.com/fogatlas/crd-client-go) that model a distributed infrastructure (Region,
Link, ExernalEndpoint) and to extends a k8s Deployment, called FADepl;
1. a controller of the introduced CRDs called [fadepl-controller](https://github.com/fogatlas/fadepl-controller);
1. other components, namely:
   * a monitoring system based on a vanilla Prometheus plus customized exporters
    in order to measure network  parameters (bandwidth and latency) of a distributed
    fog infrastructure;
   * a set of GUIs able to provide a topological view of a distributed
   infrastructure and to model and deploy a microservice-based application on that infrastructure;
   * a set of Ansible playbooks for automatically setting up a distributed physical/virtual environment based
   on OpenStack, Docker, Kubernetes and, in case of a public environment, protected with a VPN.

   These components are not publicly available at the moment.

## FogAtlas installation

For installing the Open Source components of FogAtlas, please follow the instruction
detailed [here](https://github.com/fogatlas/fadepl-controller#what-you-need-to-do-in-order-to-play-with-fadepl-controller).

For any problem, do not hesitate to open an issue.

## FogAtlas Legacy

The organization [FogAtlas legacy](https://github.com/fogatlas-legacy) contains an older
version of FogAtlas that you can check out so as to execute the _demo kit_, a tool that can
be used to play with FogAtlas in a virtual environment in order to get an idea
of the FogAtlas features.
The _demo_kit_ is not yet available for the newer version.    

## More Information

See [here](http://fogatlas.fbk.eu) for more information on FogAtlas project.


## License

Copyright 2019 FBK CREATE-NET

Licensed under the Apache License, Version 2.0 (the “License”); you may not use this file except in compliance with the License. You may obtain a copy of the License here.

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
