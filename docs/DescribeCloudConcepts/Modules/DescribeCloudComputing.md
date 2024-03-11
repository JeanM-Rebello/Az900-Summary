[Return to choice module page](https://github.com/JeanM-Rebello/Az900-Summary/blob/main/docs/DescribeCloudConcepts/DescribeCloudConcepts.md)

# Describe Cloud Computing

## 1 - What is cloud computing

Cloud computing is an IaaS (infrastructure as a service), which means that its focus is the sale and delivery of computing services such as VM's, storage, databases, networking, among others, via the internet.

Since it uses the internet as a means of both sales and delivery, it is not restricted by locations like traditional Datacenters and is more easily scalable.

---------------------------

## 2 - Describe the shared responsibility model

In the shared responsibility model, unlike the data center model in which the company is responsible for all stages of the data center's operation, such as maintenance, system updates, among other operational needs, part of the responsibility falls on the cloud provider. 

Depending on the choice of service type, Iaas, PaaS, Saas, more responsibility will fall on the cloud provider. 

Operations such as maintenance and updates for physical Host, Physical Network and Physical Datacenters are the responsibility of the cloud provider regardless of the type of service chosen, in this case specifically Azure.

Operations such as account and identity management, types and IPs of devices that will have access and what types of information and data will be stored, as well as their security, are completely responsible for the customer regardless of the type of service chosen.

--------------------

## 3 - Define cloud models

There are 3 types of cloud model:

### Private Cloud:

A private cloud can be On-Premises, meaning the virtualization of a company's own Datacenter to the cloud. Not having many advantages over other cloud models, but simplifying access to the datacenter as it now has access to a large-scale third-party network.

It can also be a cloud contracted from third parties, in a very similar way to contracting a public cloud. But unlike public clouds where the infrastructure responsibility falls on the provider, in private clouds contracted from third parties the responsibility for maintaining the physical infrastructure falls completely on the customer and only the customer's employees or authorized personnel have access to the physical part.
<br>

### Public Cloud:

The public cloud is the best-known cloud solution. This type of cloud is one in which you outsource all physical maintenance to the provider, in addition to the entire infrastructure also being owned by the provider.
<br>

### Hybrid Cloud:

The hybrid cloud is basically a mix of the two previous cloud models, an example would be a company having a local data center and wanting to migrate to the cloud without losing this investment.
With a hybrid cloud solution, they would carry out a process in which the entire local structure is connected to the provider in order to virtualize access using the provider's network, much like what we would do in a private cloud, and now because they are connected they can also contract cloud services as in a public cloud.
<br>

### Multi-Cloud:

A new situation occurring is Multi Cloud, it is increasingly common for the same company to have multiple different clouds contracted, for whatever the reasons, such as migration between clouds, the use of different resources from each cloud.

"Regardless, in a multi-cloud environment you deal with two (or more) public cloud providers and manage resources and security in both environments." <br>- Part taken from Microsoft Learn
<br>

### Azure tools:

#### Azure Arc -
Azure Arc is a Microsoft solution that extends Azure services to environments outside of the Microsoft cloud. 

It allows organizations to manage resources across on-premises, multi-cloud environments, and edge computing using the same tools, policies, and practices that would be applied in the Azure cloud.

#### Azure VMware Solution-

Azure VMware Solution is an offering from Microsoft in partnership with VMware to provide an integrated solution that allows you to run and migrate VMware virtual machines directly into Microsoft Azure. 

This solution is designed for organizations that want to leverage the benefits of the Azure public cloud without having to completely restructure their existing VMware-based infrastructure.

----------------------------

## 4 - Describe the consumption-based model

The consumption-based model in Azure refers to a flexible, pay-as-you-go pricing approach where users are billed based on their actual usage of resources and services. 

Instead of initial fixed costs, customers pay for the computing resources and services they consume, allowing greater flexibility, cost efficiency and exchanging capital expenses (CapEx), arising from the purchase and maintenance of a data center structure, for operational expenses ( OpEx) allowing greater room for maneuver for the company.

-----------
[Advance to the next module](https://github.com/JeanM-Rebello/Az900-Summary/blob/main/docs/DescribeCloudConcepts/Modules/DescribeTheBenefitsOfUsingCloudServices.md)
