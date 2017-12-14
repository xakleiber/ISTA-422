--Discussion 06

--ISTA-422

--Name: Xavier Kleiber

 - 1. What is the target of Azure SQL Databases?
	- Online transaction processing workloads.

 - 2. By default, how many logical SQL Databasae servers can you have per Azure subscription?
	- Six

 - 3. Why does the connection string set the TrustServerCertificate property to False and the Encrypt property to True?
	- This is to provide additional protection while accessing SQL Database over the Internet. Doing so helps thwart potential man-in the-middle attacks. SQL Database will force the connection to be encrypted regardless of the setting.

 - 4. What are transient errors?
	- Transient errors are errors that are intermittent and likely will be resolved if the command is retried. These errors are more common with SQL Database than with databases accessed via a local area network (LAN). This is due to the inherently unreliable network that is the Internet and the fact that as a managed service, SQL Database might periodically undergo maintenance activities that could cause connections to drop temporarily.

 - 5. What three things contribute to the total cost for running a SQL Server deployment on Azure Virtual Machines?
	- Windows Server cost
	- Azure Storage cost
	- SQL Server license cost

 - 6. Why do you need to be converned about high availability and disaster recovery for SQL Server in Azure Virtual Machines?
	- Azure provides high-availability features for the VMs, but not necessarily for SQL Server running on the VM. It is possible for the VM to be online but the SQL Server instance to be offline, unhealthy, or both. Additionally, it is possible for the VM to unavailable due to hardware failure or software upgrades. Therefore, a practiced HADR strategy should be considered.

 - 7. What are six SQL Server features tat are not currently supported in SQL Database (according to the book)?
	- Windows authentication
	- FILESTREAM data
	- Database mirroring
	- Extended stored procedures
	- SQL Server Agent/Jobs
	- SQL Server Reporting Services

 - 8. Name four factors to consider when choosing between SQL Database and SQL Server in Azure Virtual Machines.
	- Database size
	- Existing application versus new application
	- Level of administrative control
	- business continuity strategy

 - 9. Who did Microsoft collaborate with to bring ClearDb database as a service for MySQL to the Azure platform?
	- SuccessBricks

 - 10. What two options exist in Azure if you don't need a relational database management system (RDBMS)-based data storage solution sush as SQL Database or SQL Server in Azure Virtual Machinges?
	- DocumentDB
	- Azure Table storage