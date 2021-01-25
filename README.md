# Shared Service Contract and Data Contract in WCF

This article describes how to create WCF ServiceContract and DataContract that can be shared to multiple assemblies or WCF services and clients. 

In many scenarios sharing of WCF, contract is useful like if you multiple WCF service assemblies that shared service contracts and data contracts or if you want to create a wrapper that would instantiate service proxies or you want to have dynamic creation of service proxies using ChannelFactory to avoid ServiceContract changes issues.

We will follow the below steps to create Service Contract and Data Contract that can be shared in multiple assemblies.

## Projects

1. [NorthwindContracts](https://github.com/geeksarray/shared-service-contract-and-data-contract-in-wcf/tree/main/NorthwindDynamicProxy/NorthwindContracts) - WCF Service and Data Contracts that are shared with multiple WCF services.

1. [NorthwindServices](https://github.com/geeksarray/shared-service-contract-and-data-contract-in-wcf/tree/main/NorthwindDynamicProxy/NorthwindServices) - WCF Service assembly having Product and Category Service using DataContract and ServiceContract from NorthwindContracts project.

ProductService host will be like this

![WCF Service and Data Contracts shared in multiple services](https://geeksarray.com/images/blog/ProductService.png)

For more detailed steps and description please visit - https://geeksarray.com/blog/shared-service-contract-and-data-contract-in-wcf
