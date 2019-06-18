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

* [€30 for first computer to €5000 for unlimited enterprise use](https://www.ssmstoolspack.com/Licensing)


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

I don't know about you but one less reason to fire up the Windows VM sure does
make me happy. Combined with dotnet core I haven't fired up Windows in months
now.


## Cross-database

### Razor Sql

![Razor Sql Screenshot](https://www.razorsql.com/images/razorsql/main45.jpg){:height="200px"}

<http://www.razorsql.com/>

### EZ Data Browser

![EZ Data Browser Screenshot](http://www.softimum-solutions.com/Content/Images/Overview.png){:height="200px"}

<http://www.softimum-solutions.com/Data-Browser/Overview.aspx>

* $29.99 per computer
* Licence key by email
* pay via PayPal of credit card

## Unsorted (wip)

* <http://sqleo.sourceforge.net/> - <https://www.youtube.com/watch?v=emDrdj0IxNI>
* <http://sqlfiddle.com/>
* <http://www.dbschema.com/sqlite-designer-tool.html>
* <http://www.magereverse.com/>
* <http://www.sqlservercentral.com/articles/Tools/157911/>
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
* intellij/rider/rubymine etc all have the datagrip capabilities built in
* razorsql
* redgate sql prompt

## Places to find even more database tools

* <https://en.wikipedia.org/wiki/Comparison_of_database_tools>
* <https://www.quora.com/How-do-I-generate-an-entity-relationship-diagram-for-a-SQLite-database-file?share=1>
* <https://www.quora.com/What-are-some-good-online-database-schema-design-tool-with-larger-days-of-expiry>
* <https://alternativeto.net/software/mysql-workbench/>

## The end

I hope you found at least a few you didn't know about and that they make your life better in some way. Please do tell me the story of how this helped you on [email](tim@schemaexplorer.io) or [twitter](https://twitter.com/tim_abell).
Did I miss something? If you wish to improve this article please ping me a PR with additions here: https://github.com/timabell/sdv-website or just [email me](tim@schemaexplorer.io).

I'm not being paid to promote these, these are not affiliate links, I share this learning with you all for free so that we can all enjoy our work with databases more, and create better more reliable databases for ourselves, our clients and our projects.

If you want to be notified of new articles, sign up to the mailing list (which currently is also the trial download list).

Till next time!