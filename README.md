# DP-203
prepartion for DP-203 Certification


Understanding Data
=> Classification of data 
1.structured data (represented by rows and col)
2.semi-strutured data( represented by JSON)
3.unstructed Data(Image,videos)

#### Task 1: .net application being able to fetch an Azure SQL database and an Azure storage account.
the images data within the application itself.You need to have different storage locations
for data storage.Idly have one data store for storing that CSV based information and maybe another data store for storing the images.

 
 **🔊Note**: the usage of a service known as an Azure storage account, which we will use for storing the images, and an Azure SQL database for storing the application data.
Please note that you could store your images and the data.csv file hazardous in the Azure storage account.We don't need the SQL database, but since you wanna look at the relational aspects of a database engine,I'm going forward with the implementation
of the Azure SQL database.

## Azure storage Accounts( Store of data in the cloud) 
-> it is a service on Azure platform
different services: 
  1. Table service: where you can actually store structured NoSQL data.So, for example, if you wanna host, you know,tables within the Azure storage account you can make use of the Table service.
  2. bolb service: this is object storage , when it comes onto the Azure storage account.(This means that anything that you upload to the service,
  so you could upload a file onto the service.That file is treated as a binary object.This service is good when you want to upload objects such as your audio files, your video files, images etc.
  3. File services: If you want to just have a file share in place,you know, you could have file shares that could be connected onto different systems. You can make use of the File service in the Azure storage account.
  4. Queue service: If you have messages that need to be sent by different components of a distribute application, you can make use of the Queue service.
     
#### Microsoft Sql Server :
Microsoft SQL Server can be used through the Azure SQL Database service, where the underlying server management is handled for you. This service includes database software with features like high availability, automatic backups, and restore options. It allows you to easily host your databases.


#### Storage account endpoints
A storage account provides a unique namespace in Azure for your data. Every object that you store in Azure Storage has a URL address that includes your unique account name. The combination of the account name and the service endpoint forms the endpoints for your storage account.

#### Example udemy 
data analysis of udemy -> where it needs to store the videos , descripition of the video ,ratings and the price.
Udemy needs to store structured information about courses, instructors, ratings, and prices, potentially in a relational database. Video content could be stored using Azure Blob storage. Additionally, Udemy must analyze data on student purchases to enhance services and improve the platform. This chapter encourages understanding the various aspects of data storage, usage, and analysis in applications.

## Azure Data Lake Gen2 Storage Account.
Azure Data Lake Storage Gen2 is a set of capabilities built on Azure Blob Storage, designed for big data analytics. It merges the features of Azure Data Lake Storage Gen1 with Blob Storage, providing file system semantics, file-level security, scalability, low-cost tiered storage, and high availability/disaster recovery.

Data Lake Storage Gen2 serves as the foundation for enterprise data lakes on Azure, managing petabytes of data with high throughput. A data lake is a centralized repository for storing all types of data, both structured and unstructured, in their raw formats, facilitating easy access and analysis.

