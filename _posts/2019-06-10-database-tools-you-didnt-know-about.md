---
layout: article
title: Database tools I was surprised existed
description: A complete list of tools for database people and developers
category: blog
---

But you already know all the tools for working with databases don't you?

That's what I thought too before I started working on [SQL Schema
Explorer](http://schemaexplorer.io/). Even after 18 years working with
databases it turns out I only knew a fraction of the tools that are out there.

Working on SQL Schema Explorer gave me a reason I didn't have before to search
the internet in new ways relating to databases, and now that I'm reaching out
to people about SQL Schema Explorer people are in turn sharing their favourite
tools with me.

I'd hate for this gift to sit hidden away in my private product trello board,
so I've turned it into this article so that you can skip the wilderness years
and gain a zen-like awareness of all the tools of your trade. I'm sure you
won't like or use all of them, and many overlap in function, but the following
list will allow you to try out and asses each one against your needs; perhaps
you'll find a new tool that will save you hours, or make your job that much
more enjoyable. Never again will you have to say to a new colleague "oh I
hadn't heard of that one!".

## Microsoft Sql Server

### SSMS Tools Pack

<https://www.ssmstoolspack.com/>

An add-on to management studio that improves many pieces of of ssms and adds new capabilities.

![Screenshot of CRUD generation in SSMS Tools](https://www.ssmstoolspack.com/Content/Images/Features/CRUD.png){:height="200px"}

* €30 for first computer to €5000 for unlimited enterprise use ([SSMS Toolpack
  Pricing page](https://www.ssmstoolspack.com/Licensing))

A friend of mine saved many hours using the "CRUD" stored procedure generation capabilities.

### Sql Server Management Studio (SSMS)

Okay you know this one but I have to mention it.

It has awkward but functional diagram support. You can version control these
diagrams and move them between servers with
<https://github.com/timabell/database-diagram-scm> which is worth knowing about
if you ever use the ssms diagrams.

### You can now run MSSQL on open source

Did you know Microsoft SQL Server (aka mssql) is now available on both linux
natively and in docker containers? It's the real deal, not like mono vs .net

* [SQL Server on Linux](https://docs.microsoft.com/en-us/sql/linux/sql-server-linux-setup)
* [SQL Server in Docker](https://docs.microsoft.com/en-us/sql/linux/quickstart-install-connect-docker?view=sql-server-2017)

Here's all it takes to fire up mssql, the only pre-requisite is docker itself.

	docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=your_new_sa_passwod' \
	-p 1433:1433 --name mssql1 \
	-d mcr.microsoft.com/mssql/server:2017-latest

This isn't a tool per-se, but this is too important to not mention, especially
as it's quite new and not everyone is aware of this exciting change from
redmond.

I don't know about you but one less reason to fire up the Windows VM sure does
make me happy. Combined with dotnet core I haven't fired up Windows in months
now.

## Cross-database

### Razor Sql

![Razor Sql Screenshot](https://www.razorsql.com/images/razorsql/main45.jpg){:height="200px"}

<http://www.razorsql.com/>

> "RazorSQL is an SQL query tool, database browser, SQL editor, and database
> administration tool for Windows, macOS, Mac OS X, Linux, and Solaris.
> RazorSQL has been tested on over 40 databases, can connect to databases via
> either JDBC or ODBC"

### EZ Data Browser

![EZ Data Browser Screenshot](http://www.softimum-solutions.com/Content/Images/Overview.png){:height="200px"}

<http://www.softimum-solutions.com/Data-Browser/Overview.aspx>

* $29.99 per computer
* Licence key by email
* pay via PayPal of credit card

> "software from Softimum Solutions to help users to browse and to edit SQL Server databases quickly and easily"

Provides a configurable MSAccess-like interface to a database.

### SQLeo

Cross-database query builder/analyser. Feature rich - data/schema compare, pivot queries, diagrams etc.

![SQLeo screenshot](http://sqleo.sourceforge.net/images/Pivot%20Query.PNG){:height="200px"}

* <http://sqleo.sourceforge.net/>

> "A powerful SQL tool to transform or reverse complex queries (generated by
> OBIEE, Microstrategy, Cognos, Hyperion, Pentaho ...) into diagrams to ease
> visualization and analysis. A graphical query builder that permits to create
> complex SQL queries easily. The GUI with multi-connections supports virtually
> all JDBC drivers, including ODBC bridge, Oracle, MySQL, PostgreSQL, Firebird,
> HSQLDB, H2, CsvJdbc, SQLite. And top of that, everything is open-source!"

* [SQLeo demo video on youtube](https://www.youtube.com/watch?v=emDrdj0IxNI)
* Sourceforge page (ugh) <https://sourceforge.net/projects/sqleo/>
* Fork on github <https://github.com/ojwanganto/SQLeo>


### SQL Fiddle

Live online sql editor / runner

![SQL Fiddle screenshot](/blog/img/tools/sqlfiddle-screenshot.png){:height="200px"}

* <http://sqlfiddle.com/>

### DbSchema

![DbSchema screenshot](https://www.dbschema.com/images/screenshots/database-er-diagram.png){:height="200px"}

* <http://www.dbschema.com/>

> "DbSchema is an SQL and No-SQL database designer featuring interactive
> diagrams, HTML and PDF documentation, schema versioning and migration,
> relational data browse, random data generator, visual query builder, SQL
> editor and database reports."

### DbPrompt

![DbPrompt screenshot](http://www.dbschema.com/images/dbprompt.png){:height="200px"}

* <http://www.dbschema.com/dbprompt.html>

> "Free Universal Multi-Database SQL Prompt - DbPrompt can execute queries on
> multiple databases, transfer data between databases, upload result files on
> ftp servers, execute complex SQL scripts using Java Groovy and cron-schedule
> scripts for execution and report failures per email. DbPrompt supports all
> SQL and NoSQL databases, like MySql, Cassandra, PostgreSql, MongoDb,
> Redshift, SqlServer, Azure, Oracle, Teradata and more. DbPrompt can work on
> all operating systems. DbPrompt is free of charge. "

## Unsorted - omg will it never end

* <http://www.magereverse.com/>
* <https://dataedo.com/>
* <https://dbvis.com/>
* <https://docs.microsoft.com/en-us/sql/azure-data-studio>
* <https://github.com/ajdeziel/SQL-Data-Viewer> - abandoned
* <https://github.com/preston/railroady/>
* <https://help.talend.com/reader/ISPDm8GQ6s0HN0348QulWg/Ij~7tBlW8im63rAGnGHT3A>
* <https://portableapps.com/apps/development/database_browser_portable>
* <https://redash.io/>
* <https://sequelpro.com/>
* <https://softwarerecs.stackexchange.com/questions/11346/tool-to-visualize-sql-database-schema>
* <https://sqldbm.com/en/>
* <https://sqlitestudio.pl/>
* <https://www.codediesel.com/data/5-tools-to-visualize-database-schemas/>
* <https://www.datasparc.com/>
* <https://www.dbsoftlab.com/online-tutorials/active-table-editor-online-tutorials.html>
* <https://www.devart.com/dbforge/sql/studio/>
* <https://www.idera.com/er-studio-data-architect-saftware>
* <https://www.jetbrains.com/datagrip/> - <https://www.youtube.com/watch?v=Xb9K8IAdZNg>
* <https://www.metabase.com/>
* <https://www.navicat.com/en/products/navicat-data-modeler>
* <https://www.schemacrawler.com/>
* <https://www.sqlservercentral.com/articles/microsoft-sql-server-utilities-and-tools-1>
* <https://jetbrains.com/> intellij/rider/rubymine etc all have the datagrip capabilities built in
* <https://www.red-gate.com/> sql prompt etc
* <https://www.oracle.com/database/technologies/appdev/datamodeler.html>
* <https://erwin.com/products/erwin-data-modeler/>
* DBeaver
* Azure Data Studio - PostgreSQL extension
* SAP PowerDesigner <https://www.sap.com/products/powerdesigner-data-modeling-tools.html> - I have no idea what this is. Sounds enterprisey.
  * <https://en.wikipedia.org/wiki/PowerDesigner>
* <https://www.idera.com/er-studio-enterprise-data-modeling-and-architecture-tools>
* <https://www.idera.com/er-studio-data-architect-software>
* <https://sparxsystems.com/products/ea/>
* <https://www.ibm.com/us-en/marketplace/infosphere-data-architect>
* <https://www.postgrescompare.com/>

## Places to find even more database tools and learn more

* <https://en.wikipedia.org/wiki/Comparison_of_database_tools>
* <https://www.quora.com/How-do-I-generate-an-entity-relationship-diagram-for-a-SQLite-database-file?share=1>
* <https://www.quora.com/What-are-some-good-online-database-schema-design-tool-with-larger-days-of-expiry>
* <https://alternativeto.net/software/mysql-workbench/>
* <https://www.datasciencecentral.com/profiles/blogs/top-6-data-modeling-tools>
* <https://www.educba.com/9-best-data-modeling-tools/>
* <http://www.agiledata.org/essays/dataModeling101.html> - I had no idea what data modelling really meant before reading this.
* <http://www.sqlservercentral.com/articles/Tools/157911/>
* <https://www.apgdiff.com/>
* <http://toolsfordatabases.com/>
* <https://www.webfx.com/blog/web-design/top-five-best-database-management-tools/>
* <https://solutionsreview.com/data-management/data-management-solutions-directory/>
* <https://www.softwaretestinghelp.com/tools/26-best-data-integration-tools/>


## Information overload

If you got this far you probably need to get back to work. It's clear this
article is a bit ridiculous now so I'm not going to carry on sorting it out.
The internet is littered with catalog articles of varying completeness and
quality. To make it complete and good would make it dull and endless.

Watch this space, I think I'll try and work out what people actually are trying
to do and cater for that. Maybe we can all build a collaborative index
somewhere.

## The end

I hope you found at least a few you didn't know about and that they make your
life better in some way. Please do tell me the story of how this helped you on
[email](tim@schemaexplorer.io) or [twitter](https://twitter.com/tim_abell).
Did I miss something? If you wish to improve this article please ping me a PR
with additions here: https://github.com/timabell/sdv-website or just [email
me](tim@schemaexplorer.io).

I'm not being paid to promote these, these are not affiliate links, I share
this learning with you all for free so that we can all enjoy our work with
databases more, and create better more reliable databases for ourselves, our
clients and our projects.

If you want to be notified of new articles, sign up to the mailing list (which
currently is also the trial download list).

Till next time!
