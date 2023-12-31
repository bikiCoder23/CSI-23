# CSI-23
This is my final project of Power Bi Dashboard for the Celebal Summer Internship 2023

## Project Workflow

### Data Pipeline Setup:

1. **Resource Group Creation:** Initiate by establishing a Resource group with an appropriate name to organize resources effectively.
2. **Azure Data Factory Instance:** Within the established Resource group, create an instance of Azure Data Factory. Ensure to provide essential details such as name, region, adhering to company policies.
3. **Azure Storage Account:** Establish an Azure Storage Account, specifically choosing the “Data Lake Storage Gen2” option during the setup.
4. **Azure SQL Database Setup:** Create an Azure SQL Database, ensuring the settings like SQL Authentication, server admin login, password, and necessary access permissions are appropriately configured.
5. **Container Configuration:** In the Storage account, set up a container named “ingest” to link with the client's on-premise server for data extraction.
6. **Azure Data Factory Linked Services:** Within the Azure Data Factory, craft linked services for both Azure SQL Database and Azure Data Lake Storage Gen2, ensuring correct authentication and connection details.
7. **Dataset Creation:** Develop datasets within Azure Data Factory for both SQL Database and Data Lake Storage Gen2, specifying data formats, linked services, and relevant configurations.
8. **Pipeline Creation:** Establish a pipeline within Azure Data Factory to facilitate real-time data access. Configure activities like data copying from the source (Data Lake Storage) to the destination (SQL Database), with appropriate mappings.
9. **Trigger Implementation:** Incorporate triggers within the pipeline based on scheduled intervals or event-driven requirements. This ensures automated data transfer from the client's server to Celebal’s Azure Server.

### Data Transformation & Visualization:

**SQL Server Management Studio Access:** Utilize SQL Server Management Studio to access the Azure SQL server created previously. Ensure to authenticate using the credentials set during the SQL Server configuration.
**Data Cleansing & Transformation:** Employ SQL queries within the SQL Server Management Studio to transform the pipelined data, focusing on data cleansing or scrubbing as specified.
**Dashboard Creation in Power BI:** Post transformation, import the processed data into Power BI from SQL Server. Here, design an interactive and dynamic dashboard, presenting data insights in a visually appealing and actionable manner, guiding future decision-making processes.
