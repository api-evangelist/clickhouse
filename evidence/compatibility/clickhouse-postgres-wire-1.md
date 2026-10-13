<!-- fetched 2026-10-13 from https://clickhouse.com/docs/interfaces/postgresql by sweep-shape-compat.py; text extracted from the provider's own page -->

. -->
 PostgreSQL interface - ClickHouse Documentation 
 Documentation Index
 Fetch the complete documentation index at: /docs/llms.txt 
 Use this file to discover all available pages before exploring further.
 Skip to main content ClickHouse Documentation home page 
 Search...
 ⌘ K 
 Overview 
 Fundamentals 
 Core concepts 
 Glossary 
 Table parts 
 Table partitions 
 Part merges 
 Primary indexes 
 Query parallelism 
 Architecture overview 
 ClickHouse concepts 
 Overview 
 Materialized views 
 Dictionaries 
 Projections 
 Performance 
 Operations 
 Configuration 
 Security and auth 
 Backup and restore 
 Interfaces 
 Native Clients and Interfaces 
 clickhousectl 
 ClickHouse Client 
 Model Context Protocol (MCP) 
 Drivers and interfaces 
 Overview 
 HTTP interface 
 Framing formats 
 Native interface (TCP) 
 ADBC driver 
 MySQL interface 
 ODBC driver 
 PostgreSQL interface 
 Prometheus API and PromQL 
 Prometheus metrics endpoint 
 SSH interface 
 gRPC interface 
 Arrow Flight interface 
 Schema inference 
 Documentation Search 
 Web SQL UI 
 SQL Console 
 Web UI Color Coding 
 Web UI Pinned Columns 
 Web UI Notebook Mode 
 Web UI Result Shaping 
 Web Terminal 
 Third-party clients 
 Tools and utilities 
 Best practices 
 Best practices in ClickHouse 
 Choosing a primary key 
 Selecting data types 
 Use materialized views 
 Minimize and optimize JOINs 
 Choosing a partitioning key 
 Selecting an insert strategy 
 Data skipping indices 
 Avoid mutations 
 Avoid optimize final 
 Avoid nullable columns 
 Using JSON 
 English 
 Home 
 Database 
 Solutions 
 Integrations 
 Resources 
 ClickHouse Documentation home page English 
 Search...
 ⌘ K 
 Search... 
 Navigation 
 Drivers and interfaces 
 PostgreSQL interface
 Home 
 Database 
 Solutions 
 Integrations 
 Resources 
 ClickHouse concepts 
 Interfaces 
 Drivers and interfaces
 PostgreSQL interface
 Documentation for the PostgreSQL wire protocol interface in ClickHouse
 Check out our ClickHouse Managed Postgres service. Backed by NVMe storage that is physically collocated with compute, it delivers up to 10x faster performance for workloads that are disk-bound compared to alternatives using network-attached storage like EBS and allows you to replicate your Postgres data to ClickHouse using the Postgres CDC connector in ClickPipes. 
 ClickHouse supports the PostgreSQL wire protocol, which allows you to use Postgres clients to connect to ClickHouse. In a sense, ClickHouse can pretend to be a PostgreSQL instance - allowing you to connect a PostgreSQL client application to ClickHouse that isn’t already directly supported by ClickHouse (for example, Amazon Redshift). 
 To enable the PostgreSQL wire protocol, add the postgresql_port setting to your server’s configuration file. For example, you could define the port in a new XML file in your config.d folder: 
 < clickhouse > 
 < postgresql_port > 9005 </ postgresql_port > 
 </ clickhouse > 
 Startup your ClickHouse server and look for a log message similar to the following that mentions Listening for PostgreSQL compatibility protocol : 
 {} <Information> Application: Listening for PostgreSQL compatibility protocol: 127.0.0.1:9005 
 ​ 
 Connect psql to ClickHouse 
 The following command demonstrates how to connect the PostgreSQL client psql to ClickHouse: 
 psql -p [port] -h [hostname] -U [username] [database_name] 
 For example: 
 psql -p 9005 -h 127.0.0.1 -U alice default 
 The psql client requires a login with a password, so you won’t be able connect using the default user with no password. Either assign a password to the default user, or login as a different user. 
 The psql client prompts for the password: 
 Password for user alice: 
 psql (14.2, server 22.3.1.1) 
 WARNING: psql major version 14, server major version 22. 
 Some psql features might not work. 
 Type "help" for help. 
 default=> 
 And that’s it! You now have a PostgreSQL client connected to ClickHouse, and all commands and queries are executed on ClickHouse. 
 The PostgreSQL protocol currently only supports plain-text passwords. 
 ​ 
 Using SSL 
 If you have SSL/TLS configured on your ClickHouse instance, then postgresql_port will use the same settings (the port is shared for both secure and insecure clients). 
 Each client has their own method of how to connect using SSL. The following command demonstrates how to pass in the certificates and key to securely connect psql to ClickHouse: 
 psql "port=9005 host=127.0.0.1 user=alice dbname=default sslcert=/path/to/certificate.pem sslkey=/path/to/key.pem sslrootcert=/path/to/rootcert.pem sslmode=verify-ca" 
 ​ 
 Configuring ClickHouse user authentication with SCRAM-SHA-256 
 To ensure secure user authentication in ClickHouse, it is recommended to use the SCRAM-SHA-256 protocol. Configure the user by specifying the password_scram_sha256_hex element in the users.xml file. The password hash must be generated with num_iterations=4096. 
 Ensure that the psql client supports and negotiates SCRAM-SHA-256 during connection. 
 Example configuration for user user_with_sha256 with the password abacaba : 
 < user_with_sha256 > 
 < password_scram_sha256_hex > 04e7a70338d7af7bb6142fe7e19fef46d9b605f3e78b932a60e8200ef9154976 </ password_scram_sha256_hex > 
 </ user_with_sha256 > 
 View the PostgreSQL docs for more details on their SSL settings. 
 Last modified on July 24, 2026
 Was this page helpful?
 Yes No 
 Suggest edits Raise issue 
 Previous Prometheus API and PromQL
 Prometheus HTTP API support in ClickHouse: remote write, remote read, and PromQL queries over a TimeSeries table. 
 Next 
 ⌘ I 
 On this page 
 Connect psql to ClickHouse 
 Using SSL 
 Configuring ClickHouse user authentication with SCRAM-SHA-256 
 Copy page View as Markdown Download PDF Set up the ClickHouse documentation MCP server
