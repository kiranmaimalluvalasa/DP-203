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

## Azure Synapse service.
use : storing your data warehouse 

Azure SQL Database is a fully managed relational database service optimized for transactional workloads and general-purpose applications. It supports /*OLTP(online transaction processing)*/ scenarios with traditional SQL Server-based architecture, offering scalability through vertical and horizontal scaling. 

Azure SQL Data Warehouse (Azure Synapse Analytics) is a cloud-based data warehouse service designed for analytical processing and big data analytics. It utilizes massively parallel processing (MPP) architecture for scalable query performance across large datasets, making it ideal for /*OLAP(online analytical processing)*/  workloads and complex analytics tasks.
#### example: 
A data warehouse is a repository that can be used to store structured data .
you can use the sql query lang to work with the data in the data warehouse. by why sql ? 
online course platfrom as web application .this use a sql database
-> course
-> student 
-> order 
This is an online transaction processing system where transactions are continually added to the database, particularly on a popular platform where purchases occur frequently. However, for strategic decision-making and business insights, such as improving user experiences or forecasting market trends, senior management requires analysis of both current and historical transactional data. To avoid overloading the transactional system, which is optimized for real-time transactions, organizations use a SQL data warehouse. Unlike transactional databases, SQL data warehouses are designed for online analytical processing (OLAP), handling large datasets and supporting complex queries across historical and current data sources without impacting operational systems.


## what is difference between olap and oltp in azure

Online analytical processing (OLAP) is a technology that organizes large business databases and supports complex analysis. It can be used to perform complex analytical queries without negatively affecting transactional systems.

The databases that a business uses to store all its transactions and records are called online transaction processing (OLTP) databases. These databases usually have records that are entered one at a time. Often they contain a great deal of information that is valuable to the organization. The databases that are used for OLTP, however, were not designed for analysis. Therefore, retrieving answers from these databases is costly in terms of time and effort. OLAP systems were designed to help extract this business intelligence information from the data in a highly performant way. This is because OLAP databases are optimized for heavy read, low write workloads.

### Microsoft Entra Id and permissions

Microsoft Entra ID: When you create an Azure account, you get Microsoft Entra ID (formerly Azure Active Directory), which manages user authentication and authorization.
User Roles: In Microsoft Entra ID, you can create different users and assign them roles. For example, in a company, different users need access to different resources in Azure.

###### Role-Based Access Control (RBAC):
Assigning Roles: You assign roles to users to control what they can access. There are built-in roles like contributor, owner, and reader.
Storage Blob Data Reader Role: We assigned this role to our Azure admin user to allow reading data from storage blobs. This role has specific permissions needed for accessing the data.

### what is difference btwn dedicated sql pool and serverless sql pool
### what is difference betwwen dedicated external sql pool and dedicated sql pool 
we can create the external tables in dedicated sql pool and serverless sql pool - > why we need to create the external tables ?

## Data warehouse:
split into Fact and Dimension tables
these tables either conform onto a star or snowflake schema
Fact tables are meant to store quantitative data, this a data that can be measured


