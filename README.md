# DP-203
prepartion for DP-203 Certification


Understanding Data
=> Classification of data 
1.structured data (represented by rows and col)
2.semi-strutured data( represented by JSON)
3.unstructed Data(Image,videos)

task 1: .net application being able to fetch an Azure SQL database and an Azure storage account.
the images data within the application itself.You need to have different storage locations
for data storage.Idly have one data store for storing that CSV based information and maybe another data store for storing the images.

 
 🔊Note: the usage of a service known as an Azure storage account, which we will use for storing the images, and an Azure SQL database for storing the application data.
Please note that you could store your images and the data.csv file hazardous in the Azure storage account.We don't need the SQL database, but since you wanna look at the relational aspects of a database engine,I'm going forward with the implementation
of the Azure SQL database.

##Azure storage Accounts( Store of data in the cloud) -> it is a service on Azure platform
different services: 

  1.bolb service: this is object storage , when it comes onto the Azure storage account.(This means that anything that you upload to the service,
  so you could upload a file onto the service.That file is treated as a binary object.This service is good when you want to upload objects such as your audio files, your video files, images etc.
  
  2. Table service: where you can actually store structured NoSQL data.So, for example, if you wanna host, you know,tables within the Azure storage account you can make use of the Table service.
  3. File services: If you want to just have a file share in place,you know, you could have file shares that could be connected onto different systems. You can make use of the File service
in the Azure storage account.
  4.Queue service: If you have messages that need to be sent by different components of a distribute application, you can make use of the Queue service.
