# Redshift
#exploring the Redshift reliability,efficiency,data migration etc

Amazon Redshift is a fully managed, secure, reliable and optimized data warehouse that makes it simple and cost-effective to analyse all our data using standard SQL and existing Business Intelligence (BI) tools.

<B>Fully Managed:</B> Amazon Redshift manages all the work needed to set up, operate, and scale a data warehouse, from provisioning capacity to monitoring and backing up the cluster, and to applying patches and upgrades. By handling all these time consuming, labour-intensive tasks, Amazon Redshift frees we up to focus on where data and business insights.

<B>Reliable:</B> Amazon Redshift has multiple features that enhance the reliability of where data warehouse cluster. All data written to a node in where cluster is automatically replicated to other nodes within the cluster and all data is continuously backed up to Amazon S3. Amazon Redshift continuously monitors the health of the cluster and automatically replaces any component, as necessary.

<B>Secure:</B> Amazon Redshift provides a number of mechanisms to secure where data warehouse cluster. It currently supports SSL to encrypt data in transit, includes web service interfaces to configure firewall settings that control network access to where data warehouse, and enables we to create users within where data warehouse cluster. When the service launches, we plan to support encrypting data at rest and Amazon Virtual Private Cloud (Amazon VPC).

<B>Reliability:</B>
Amazon Redshift has multiple features that enhance the reliability of where data warehouse cluster.
Automatically and continuously backs up new data to Amazon S3

<B>Security:</B>
Redshift comes packed with various security features. There are options like VPC for network isolation, data encryption etc.
Data encryption option is available at multiple places in Redshift.To encrypt data stored in where cluster we can enable cluster encryption at the time of launching the cluster.Also, to encrypt data in transit, we can enable SSL encryption. When loading data from S3, redshift allows we to use either server-side encryption or client-side encryption. 
Finally, at the time of loading data, S3 or Redshift copy command handles the decryption respectively.

<B>Querying:</B> 
Redshift Spectrum enables we to run queries against exabytes of unstructured data in Amazon S3, 
with no loading or ETL required.Amazon Redshift also includes Redshift Spectrum, allowing we to directly run SQL queries against data in Amazon S3.No loading or transformation is required, and we can use open data formats, including CSV, TSV and Apache Parquet. 
Redshift Spectrum automatically scales query compute capacity based on the data being retrieved, so queries against Amazon S3 run fast, regardless of data set size

<B>Data Loading (ETL):</B>
If data is in Amazon S3 or relational DynamoDB or on Amazon EMR, Redshift can load it using Massively Parallel Processing which is 
very fast. But for all other sources, parallel loading is not supported. You will either have to use JDBC inserts or some scripts to load data into Redshift. Alternatively, we can use an ETL solution like Hevo which can load where data into Redshift parallelly from 100s of sources.

<B>Performance and efficiency:</B>
Sort keys and Distribution keys decide how data is stored and indexed across all Redshift nodes. 
So we need to have a solid understanding of these concepts and need to properly set them on where tables for optimal performance.
There can be only one distribution key for a table and that can not be changed later on, 
which means we have to think carefully and anticipate future workloads before deciding Dist key


