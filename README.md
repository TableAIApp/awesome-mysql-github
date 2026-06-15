# Awesome MySQL

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A hand-picked collection of mature, useful, and actively valuable tools for working with MySQL and MySQL-compatible databases.

This list focuses on practical software: clients, monitoring tools, backup utilities, schema migration systems, high-availability components, proxies, security tools, connectors, and operational toolkits.

> Maintained by the [TableAI](https://tableai.org) team.

## Contents

- [Analysis & Monitoring](#analysis--monitoring)
- [Backup & Recovery](#backup--recovery)
- [Benchmarking](#benchmarking)
- [Connectors & Drivers](#connectors--drivers)
- [Database Clients & GUIs](#database-clients--guis)
- [Development & Migrations](#development--migrations)
- [High Availability](#high-availability)
- [Proxy & Routing](#proxy--routing)
- [Security & Privacy](#security--privacy)
- [Server Distributions](#server-distributions)
- [Sharding & Scale-Out](#sharding--scale-out)
- [Toolkits & Utilities](#toolkits--utilities)

## Analysis & Monitoring

Tools for inspecting performance, understanding query behavior, monitoring servers, and analyzing MySQL internals.

- [Anemometer](https://github.com/box/Anemometer) - Web-based slow query reporting and visualization tool originally built at Box.
- [Dolphie](https://github.com/charles-001/dolphie) - Modern terminal dashboard for live MySQL, MariaDB, and ProxySQL observability.
- [innodb-ruby](https://github.com/jeremycole/innodb_ruby) - Ruby toolkit for exploring and decoding InnoDB storage files.
- [innotop](https://github.com/innotop/innotop) - Classic terminal monitor for MySQL activity, replication, locks, and server health.
- [MySQL Explain Analyzer](https://github.com/Preetam/explain-analyzer) - Web tool for reading and interpreting `EXPLAIN FORMAT=JSON` query plans.
- [MySQLTuner-perl](https://github.com/major/MySQLTuner-perl) - Widely used command-line advisor for reviewing MySQL configuration and server health.
- [Percona Monitoring and Management](https://github.com/percona/pmm) - Full monitoring and management platform for MySQL, MongoDB, PostgreSQL, and related infrastructure.
- [Prometheus mysqld_exporter](https://github.com/prometheus/mysqld_exporter) - Prometheus exporter for collecting MySQL server metrics.
- [pstop](https://github.com/sjmudd/ps-top) - `top`-style performance monitor powered by MySQL Performance Schema.
- [Wireshark](https://gitlab.com/wireshark/wireshark/) - Network protocol analyzer with support for inspecting MySQL traffic.

## Backup & Recovery

Reliable tools for logical backups, physical backups, restore workflows, and disaster recovery.

- [Dumpling](https://github.com/pingcap/tidb/tree/master/dumpling) - High-performance logical export tool for MySQL and TiDB, designed for parallel dumping.
- [MyDumper](https://github.com/mydumper/mydumper) - Fast parallel logical backup and restore utility for MySQL-compatible databases.
- [Percona XtraBackup](https://github.com/percona/percona-xtrabackup) - Production-grade physical hot backup tool for MySQL and Percona Server.
- [UnDROP for InnoDB](https://github.com/twindb/undrop-for-innodb) - Recovery toolkit for extracting data from damaged or dropped InnoDB tablespaces.

## Benchmarking

Tools for load testing, stress testing, and measuring MySQL performance under realistic workloads.

- [go-tpc](https://github.com/pingcap/go-tpc) - Go implementation of TPC-C and TPC-H style benchmarks for MySQL-compatible systems.
- [HammerDB](https://github.com/TPC-Council/HammerDB) - Open-source database benchmarking suite supporting MySQL and many other databases.
- [iibench-mysql](https://github.com/tmcallaghan/iibench-mysql) - Java implementation of the Index Insertion Benchmark for MySQL, MariaDB, and Percona Server.
- [Sysbench](https://github.com/akopytov/sysbench) - Popular multi-threaded benchmarking tool for database, CPU, memory, file I/O, and mutex workloads.

## Connectors & Drivers

Stable client libraries and database drivers for connecting applications to MySQL and compatible servers.

- [DBD::MariaDB](https://github.com/perl5-dbi/DBD-MariaDB) - Perl DBI driver for MariaDB and MySQL.
- [DBD::mysql](https://github.com/perl5-dbi/DBD-mysql) - Perl DBI driver for MySQL.
- [go-sql-driver/mysql](https://github.com/go-sql-driver/mysql) - Mature MySQL driver for Go's standard `database/sql` package.
- [MariaDB Connector/J](https://github.com/mariadb-corporation/mariadb-connector-j) - Java client library for MariaDB and MySQL-compatible databases.
- [MySQL C API](https://dev.mysql.com/downloads/c-api/) - Official C client library for MySQL.
- [MySQL Connector/C++](https://github.com/mysql/mysql-connector-cpp) - Official MySQL driver for C and C++ applications.
- [MySQL Connector/J](https://github.com/mysql/mysql-connector-j) - Official JDBC driver for Java applications.
- [MySQL Connector/NET](https://github.com/mysql/mysql-connector-net) - Official MySQL driver for .NET applications.
- [MySQL Connector/Node.js](https://github.com/mysql/mysql-connector-nodejs) - Official MySQL driver for Node.js.
- [MySQL Connector/Python](https://github.com/mysql/mysql-connector-python) - Official MySQL driver for Python.
- [mysqlclient](https://github.com/PyMySQL/mysqlclient) - Fast Python MySQL driver built on top of the MySQL/MariaDB C client library.
- [mysqljs/mysql](https://github.com/mysqljs/mysql) - Well-known pure JavaScript MySQL client for Node.js.
- [PHP mysqlnd](https://www.php.net/manual/en/book.mysqlnd.php) - Native MySQL driver included with PHP.
- [PyMySQL](https://github.com/PyMySQL/PyMySQL) - Pure Python MySQL client library.
- [Ruby mysql2](https://github.com/brianmario/mysql2) - MySQL driver commonly used in Ruby and Rails applications.

## Database Clients & GUIs

Desktop, web, and terminal clients for querying, browsing, editing, and administering MySQL databases.

- [DBeaver](https://github.com/dbeaver/dbeaver/) - Cross-platform database client with broad SQL and NoSQL support.
- [TableAI](https://tableai.org/) - MySQL client for mac with a clean UI and AI database agent.
- [Adminer](https://github.com/vrana/adminer/) - Lightweight web-based database administration tool packaged as a single PHP file.
- [HeidiSQL](https://github.com/HeidiSQL/HeidiSQL) - Long-running Windows GUI client for MySQL, MariaDB, PostgreSQL, SQL Server, and SQLite.
- [mycli](https://github.com/dbcli/mycli) - Terminal MySQL client with autocompletion, syntax highlighting, and quality-of-life improvements.
- [MySQL Shell](https://github.com/mysql/mysql-shell/) - Official advanced command-line shell for MySQL development, scripting, and administration.
- [MySQL Workbench](https://github.com/mysql/mysql-workbench) - Official visual tool for SQL development, data modeling, and MySQL administration.
- [phpMyAdmin](https://github.com/phpmyadmin/phpmyadmin) - Classic web-based MySQL and MariaDB administration interface.
- [pspg](https://github.com/okbob/pspg) - Feature-rich pager for tabular query output, useful with MySQL command-line workflows.
- [Sequel Ace](https://github.com/Sequel-Ace/Sequel-Ace) - Native macOS database client focused on MySQL and MariaDB.
- [SQLyog Community](https://github.com/webyog/sqlyog-community) - Community edition of the SQLyog MySQL GUI for Windows.
- [WebDB](https://github.com/WebDB-App/app) - Modern open-source database IDE with schema browsing, query editing, ER diagrams, and AI-assisted features.

## Development & Migrations

Tools for schema changes, database versioning, SQL review, and safer development workflows.

- [dbsafe](https://github.com/nethalo/dbsafe) - Safety checker for reviewing MySQL DDL and DML before execution.
- [Flyway](https://github.com/flyway/flyway) - Popular database migration tool for versioning and applying schema changes.
- [gh-ost](https://github.com/github/gh-ost/) - GitHub's online schema migration tool for MySQL with minimal locking.
- [Liquibase](https://github.com/liquibase/liquibase) - Database change management system for tracking, reviewing, and applying schema changes.
- [Skeema](https://github.com/skeema/skeema) - Declarative schema management tool for MySQL and MariaDB using plain SQL files.
- [SQLE](https://github.com/actiontech/sqle/blob/main/README_en.md) - SQL auditing and governance platform for development and DBA workflows.
- [test_db](https://github.com/datacharmer/test_db) - Sample MySQL database commonly used for demos, testing, and benchmarking examples.

## High Availability

Tools and systems for failover, replication management, clustering, and resilient MySQL deployments.

- [Galera Cluster](https://github.com/codership/galera) - Synchronous multi-primary clustering technology used by MariaDB Galera Cluster and Percona XtraDB Cluster.
- [Orchestrator](https://github.com/openark/orchestrator) - Battle-tested MySQL replication topology manager and automated failover system.
- [replication-manager](https://github.com/signal18/replication-manager) - High-availability and replication management platform for MySQL, MariaDB, and Percona Server.

## Proxy & Routing

Middleware for routing, pooling, failover, query control, and scaling MySQL traffic.

- [MySQL Router](https://dev.mysql.com/doc/mysql-router/en/) - Official lightweight router for MySQL InnoDB Cluster and MySQL application traffic.
- [ProxySQL](https://github.com/sysown/proxysql) - High-performance MySQL proxy with query routing, caching, multiplexing, and failover features.

## Security & Privacy

Tools for protecting data, reducing exposure, anonymizing dumps, and improving access control.

- [Acra](https://github.com/cossacklabs/acra) - Database protection suite with encryption, masking, intrusion detection, and secure data access patterns.
- [myanon](https://github.com/ppomes/myanon) - Streaming anonymizer for MySQL dumps with deterministic hashing, fixed replacements, JSON support, and custom extensions.
- [myldapsync](https://github.com/6eh01der/myldapsync) - Utility for synchronizing MySQL or MariaDB users from LDAP directories.

## Server Distributions

Mature MySQL-compatible servers and major database engines that speak the MySQL protocol.

- [MariaDB Server](https://github.com/MariaDB/server) - Community-developed MySQL fork with its own storage engines, optimizer work, and ecosystem.
- [MySQL Server](https://github.com/mysql/mysql-server) - Official Oracle MySQL server source code.
- [Percona Server for MySQL](https://github.com/percona/percona-server) - Enhanced MySQL-compatible server distribution with performance, observability, and operational improvements.
- [TiDB](https://github.com/pingcap/tidb) - Distributed SQL database with MySQL protocol compatibility and HTAP capabilities.

## Sharding & Scale-Out

Tools and platforms for running MySQL at large scale.

- [Vitess](https://github.com/vitessio/vitess) - Cloud-native database clustering system for horizontal scaling of MySQL.
- [Jetpants](https://github.com/tumblr/jetpants) - Automation toolkit for managing large sharded MySQL topologies.

## Toolkits & Utilities

General-purpose libraries, command-line tools, and operational utilities for MySQL power users.

- [go-mysql](https://github.com/go-mysql-org/go-mysql) - Go library for working with the MySQL protocol, replication streams, binlogs, and related internals.
- [Percona Toolkit](https://github.com/percona/percona-toolkit) - Essential collection of advanced command-line tools for MySQL administration, diagnostics, cleanup, and maintenance.
- [sql-splitter](https://github.com/HelgeSverre/sql-splitter) - Fast CLI for splitting, validating, sampling, converting, and working with large SQL dump files.

## Inclusion Criteria

Projects should be useful for real MySQL or MySQL-compatible database workflows.

A good fit for this list usually means:

- Mature enough for practical use
- Publicly available
- Actively useful to developers, DBAs, or data teams
- Clearly related to MySQL, MariaDB, Percona Server, TiDB, Vitess, or MySQL-compatible tooling

Small experiments, abandoned demos, thin wrappers, and purely promotional projects may be declined.
