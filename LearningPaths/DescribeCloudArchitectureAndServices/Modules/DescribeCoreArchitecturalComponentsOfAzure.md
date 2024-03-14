[Return to learning path page]()

# Describe core architectural components of azure

## 1 - What is Microsoft Azure

Microsoft Azure is a cloud computing platform and services provided by Microsoft. It offers a wide range of cloud services, including computing, storage, networking, databases, artificial intelligence (AI), Internet of Things (IoT), and more. Azure enables organizations to build, deploy, and manage applications and services in a flexible, scalable, and cost-effective manner.

---------

## 2 - Describe Azure physical infrastructure

Azure's physical infrastructure refers to the global network of data centers and supporting infrastructure owned and operated by Microsoft to deliver its cloud computing services.

Here are the key points regarding Azure's physical infrastructure:

* **Regions:**
Azure Regions refer to geographic locations where Microsoft Azure DataCenters are located, in a region there is at least 1 DataCenter available, with typically there being 3 DataCenters per region.

It is important to know which region is best for your purpose, as you need to choose the region where your resource will be. 
This choice directly impacts a series of issues ranging from cost to the appropriate functionality of the resource.

* **Availability Zones:**
Azure Availability Zones are unique physical locations within an Azure region that are equipped with independent power, cooling, and networking infrastructure, essentially DataCenters.

It is important to be able to distinguish Regions and availability zones, as they are the focal points in redundancy issues.

* **Region Pair:**
Azure region pairs are strategically paired data center locations in the same geography, typically located in the same geopolitical region or close to each other. 
Azure region pairs are primarily designed to provide geographic redundancy and enable disaster recovery, but they are also commonly used for data backup and replication purposes.

There are exceptions like Brazil which is paired unidirectionally with US because the lack of another region nearby.

* **Sovereign Regions:**
Sovereign regions in Azure refer to data center locations specifically designed to meet the data residency and compliance requirements of government and regulated industries.

Some known sovereign regions are in the USA, China and Germany.

-----------------
## Important knowledge

### **Types of Redundancy** <br><br>

**Local Redundancy:** 
Local redundancy, also known as **LRS** (Locally Redundant Storage), replicates data within a single DataCenter. 
Azure stores multiple copies of your data within the same DataCenter across different storage nodes. 
This redundancy protects against hardware failures and ensures data availability within the same data center.

**Zone Redundancy:** 
Zone redundancy, also known as **ZRS** (Zone Redundant Storage), replicates data across multiple availability zones within the same region.
Availability zones are physically separate DataCenters with independent power, cooling, and networking infrastructure. 
Zone redundancy provides higher resilience and protection against localized failures by ensuring data availability across multiple zones.

**Geo-Redundancy:** 
Geo-redundancy, also known as **GRS**(Geo-Redundant Storage), replicates data asynchronously to a secondary region located hundreds of miles away from the primary region.
In the event of a regional outage or disaster, data can be failed over to the secondary region to maintain availability and data integrity. 
Geo-redundancy provides the highest level of data protection and disaster recovery capability.

**Read-Access Locally Redundant Storage:**
Read-access Locally Redundant Storage, also known as **LA-LRS**, is similar to LRS but includes the option for hot and cool access tiers.

**Read-Access Geo-Redundancy:**
Read-access geo-redundancy, also known as **RA-GRS**, is an extension of geo-redundancy that allows read-only access to replicated data in the secondary region. This enables applications to read data from the secondary region for disaster recovery, reporting, or analytics purposes while maintaining data consistency and integrity.

------

## 3 - Describe Azure management infrastructure

The Azure account system is a comprehensive framework provided by Microsoft Azure for managing access, billing, and resources within the Azure cloud environment. Here are the key components and functions:

* **Azure Account:** 
Represents the overall relationship between the user or organization and Microsoft Azure. 
It serves as the gateway for accessing Azure services and resources.
<br>
* **Subscription:** 
Similar to the idea of an Azure sub-account linked to the main account, which is capable of containing user-provisioned resources and services.
Subscriptions are billing-related and provide access to Azure services based on your chosen pricing plans.
And it is possible to have multiple subscriptions per account, with 10 being the standard number for the Pay-As-You-Go model, but it is possible to increase this value.
<br>
* **Resource Groups:** 
Logical containers that organize related Azure resources for management purposes. Resource groups allow users to group resources, apply tags, and manage access control at the resource group level.
<br>
* **Resource:**
Resources refer to the various services, components, and objects that users can provision and manage within the Azure cloud environment. Resources encompass a wide range of functionalities, including computing, networking, storage, databases, security, monitoring, and more.
<br>
* **Billing:** 
Azure bills users based on the resources and services consumed within their subscriptions. 
Billing is typically based on usage, resource types, and pricing tiers, and users can monitor and manage their usage and costs through the Azure portal.
<br>
* **Access Control:** 
Azure provides role-based access control (RBAC) to manage access to resources.
 Users can assign roles to individuals or groups, granting permissions to perform specific actions on resources based on their roles and responsibilities.
<br>
-------
[Advance to the next module]()