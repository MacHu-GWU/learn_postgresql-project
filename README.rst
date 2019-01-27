Basic
==============================================================================

.. contents::


Install
------------------------------------------------------------------------------

Postgresql is an open source software, you can download the installation file from the official website https://www.postgresql.org/download/.

Summary:

- Windows: download binary installation file
- MacOS: installation file / Homebrew / MacPort / Flink
- Linux: package manager

Since MacOS is the developer's favorite OS


MacOS with Homebrew
------------------------------------------------------------------------------

**Install**:

- install latest: ``brew install postgresql``
- specific version: ``brew install postgresql@11.1``, for other versions, see https://formulae.brew.sh/formula/postgresql

**Run postgresql DB**:

- run postgresql service: ``brew services start postgresql``
- stop postgresql service: ``brew services stop postgresql``
- restart postgresql service: ``brew services restart postgresql``
- list all running services: ``brew services list``

For more ``brew services`` command info, see https://github.com/Homebrew/homebrew-services

**Reference**:

- Installing and configuring PostgreSQL on macOS (OSX): https://www.elliotblackburn.com/installing-postgresql-on-macos-osx/


Create Playground Database
------------------------------------------------------------------------------

``createdb`` vs ``initdb``: ``createdb`` is just a wrapper of connecting to postgres and execute ``CREATE DATABASE`` command. ``initdb`` create a new PostgreSQL database cluster. **Usually, you need** ``createdb <dbname>``.

- ``createdb`` doc: https://www.postgresql.org/docs/11/app-createdb.html
- ``initdb`` doc: https://www.postgresql.org/docs/11/app-initdb.html

**Reference**

- Creating a Database: https://www.postgresql.org/docs/current/tutorial-createdb.html


Connect to Database
------------------------------------------------------------------------------

- default host: localhost
- default port: 5432
- default username: empty
- default password: empty


psql Shell
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

``psql`` is a built-in application allows developer to use an interactive shell to talking to postgresql

- connect to database: ``psql -h <host> -p <port> -d <dbname>``
- psql command reference: https://www.postgresql.org/docs/11/app-psql.html


SQL Client Access
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
