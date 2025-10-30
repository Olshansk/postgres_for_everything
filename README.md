# Postgres for Everything (e/postgres)<!-- omit in toc -->

Keep It Simple Stupid, just use postgres. [epostgres.com](http://epostgres.com/)

## Goals & Inspiration <!-- omit in toc -->

The goal of this repository is to demonstrate how to use **Postgres for Everything**.

It's inspired by [this article](https://www.amazingcto.com/postgres-for-everything/)
from the [Amazing CTO](https://www.amazingcto.com/) as well as
[this GitHub gist](https://gist.github.com/cpursley/c8fb81fe8a7e5df038158bdfe0f06dbb)
from [@cpursley](https://gist.github.com/cpursley).

## Why maintain this list? <!-- omit in toc -->

It seems like every week I hear of a new tool on top of Postgres or another way
it can being used, so I wanted a place where I can keep track of everything. If
you have other examples, [submit a PR](https://github.com/Olshansk/postgres_for_everything/pulls).

## Star History <!-- omit in toc -->

[![Star History Chart](https://api.star-history.com/svg?repos=Olshansk/postgres_for_everything&type=Date)](https://star-history.com/#Olshansk/postgres_for_everything&Date)

## Call To Action <!-- omit in toc -->

If you have a specific code snippet, tool or project that you'll like to showcase
as an example, put up a PR with a link! Make sure to use the new [pull request template](https://github.com/Olshansk/postgres_for_everything/blob/main/.github/PULL_REQUEST_TEMPLATE.md).

## Table of Contents <!-- omit in toc -->

- [Blog Posts \& Articles](#blog-posts--articles)
- [Cron Jobs](#cron-jobs)
- [Embeddable Postgres](#embeddable-postgres)
- [Message Queues](#message-queues)
- [Analytics](#analytics)
- [GIS \& Mapping](#gis--mapping)
- [Audit Logs](#audit-logs)
- [Access Control \& Authorization](#access-control--authorization)
- [Search](#search)
  - [Full Text](#full-text)
  - [Vector](#vector)
  - [Hybrid](#hybrid)
- [Time Series](#time-series)
- [Column Oriented](#column-oriented)
- [NoSQL](#nosql)
- [Graph Data](#graph-data)
- [Foreign Data](#foreign-data)
- [HTTP](#http)
- [API Platforms](#api-platforms)
- [GraphQL and Alternative Query Languages](#graphql-and-alternative-query-languages)
- [Events, Replication, CDC](#events-replication-cdc)
- [Caching](#caching)
- [Unit Tests](#unit-tests)
- [HTML \& Applications](#html--applications)
- [Migrations](#migrations)
- [Performance Tuning](#performance-tuning)
- [Monitoring](#monitoring)
- [Scaling \& Storage](#scaling--storage)
- [User Interfaces \& Dashboards](#user-interfaces--dashboards)
- [Visualization](#visualization)
  - [Graphics Visualization](#graphics-visualization)
  - [Data Visualization](#data-visualization)
- [Package Management](#package-management)
- [Language Servers](#language-servers)
- [Data Privacy \& Security (or Data Masking)](#data-privacy--security-or-data-masking)
- [Financial Ledgers](#financial-ledgers)
- [Miscellaneous](#miscellaneous)

## Blog Posts & Articles

- [You can make Postgres scale](https://pgdog.dev/blog/you-can-make-postgres-scale)
- [Life Altering Postgresql Patterns](https://mccue.dev/pages/3-11-25-life-altering-postgresql-patterns)
- [Simplify: move code into database functions](https://sive.rs/pg)
- [Just Use Postgres for Everything](https://www.amazingcto.com/postgres-for-everything/)
- [PostgreSQL is the worlds' best database](https://www.2ndquadrant.com/en/blog/postgresql-is-the-worlds-best-database/)
- [Postgres is eating the database world](https://medium.com/@fengruohang/postgres-is-eating-the-database-world-157c204dcfc4)
- [Hacker News discussion](https://news.ycombinator.com/item?id=39273954)
- [Choose Postgres queue technology](https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology) (2023-09-24)
- [Jepsen Test on Patroni: A PostgreSQL High Availability Solution](https://www.binwang.me/2024-12-02-PostgreSQL-High-Availability-Solutions-Part-1.html) (2024-12-02)
- [PostgreSQL Full-Text Search: Fast When Done Right (Debunking the Slow Myth)](https://blog.vectorchord.ai/postgresql-full-text-search-fast-when-done-right-debunking-the-slow-myth)
- [Hacking the PostgreSQL Wire Protocol](https://pgdog.dev/blog/hacking-postgres-wire-protocol)

## Cron Jobs

- [citusdata/pg_cron](https://github.com/citusdata/pg_cron)
- [cybertec-postgresql/pg_timetable](https://github.com/cybertec-postgresql/pg_timetable)

## Embeddable Postgres

- [PGLite](https://github.com/electric-sql/pglite): WASM Postgres build packaged into a TypeScript library (< 10MB) that can run in the browser, Node.js, Bun and Deno. It's lightweight, reactive and sync live.

## Message Queues

- [tembo-io/pgmq](https://github.com/tembo-io/pgmq)
- [SKIP LOCKED](https://www.2ndquadrant.com/en/blog/what-is-select-skip-locked-for-in-postgresql-9-5/)
- [riverqueue/river](https://github.com/riverqueue/river)
- [sequinstream/sequin](https://github.com/sequinstream/sequin): Sequin is a tool for change data capture (CDC) in Postgres. Sequin makes it easy to stream Postgres rows and changes to streaming platforms and queues (e.g. Kafka and SQS). You can backfill existing rows and stream new changes in real-time.
- [janbjorge/pgqueuer](https://github.com/janbjorge/pgqueuer): PgQueuer is a Python library leveraging PostgreSQL for efficient job queuing.
- [timgit/pg-boss](https://github.com/timgit/pg-boss): pg-boss is a job queue built in Node.js

## Analytics

- [pg_analytics](https://github.com/paradedb/pg_analytics): DuckDB-powered data lake analytics from Postgres
- [pg_duckdb](https://github.com/duckdb/pg_duckdb): Official Postgres extension for DuckDB
- [BemiHQ/BemiDB](https://github.com/BemiHQ/BemiDB): Postgres read replica optimized for analytics
- [pg_moooncake](https://github.com/Mooncake-Labs/pg_mooncake): An extension for native columnstore tables in Postgres
- [Mooncake-Labs/pg_mooncake](https://github.com/Mooncake-Labs/pg_mooncake): Postgres extension that adds columnar storage and vectorized execution (DuckDB) for fast analytics within Postgres

## GIS & Mapping

- [postgis/postgis](https://github.com/postgis/postgis)

## Audit Logs

- [arkhipov/temporal_tables](https://github.com/arkhipov/temporal_tables)
- [supabase/supa_audit](https://github.com/supabase/supa_audit)
- [pgMemento/pgMemento](https://github.com/pgMemento/pgMemento)
- [pgaudit/pgaudit](https://github.com/pgaudit/pgaudit)
- [BemiHQ/Bemi](https://github.com/BemiHQ/bemi): Automatic data change tracking for PostgreSQL

## Access Control & Authorization

- [arkhipov/acl](https://github.com/arkhipov/acl)
- https://www.postgresql.org/docs/current/pgcrypto.html
- [michelp/pgjwt](https://github.com/michelp/pgjwt)
- [supabase.com/docs/guides/database/vault](https://supabase.com/docs/guides/database/vault)

## Search

### Full Text

- [Postgres Full Text Search](https://gist.github.com/cpursley/e3586382c3a42c54ca7f5fef1665be7b) (bunch of helpful links)
- [pg_search](https://github.com/paradedb/paradedb/tree/dev/pg_search): Full text search for Postgres using BM25
- [Postgres Full Text Search vs the rest](https://supabase.com/blog/postgres-full-text-search-vs-the-rest)
- [plpgsql_bm25](https://github.com/jankovicsandras/plpgsql_bm25): BM25 search implemented in PL/pgSQL

### Vector

- [pgvector/pgvector](https://github.com/pgvector/pgvector)
- [tensorchord/VectorChord](https://github.com/tensorchord/VectorChord): PostgreSQL extension designed for scalable, high-performance, and disk-efficient vector similarity search. It serves as the successor to the pgvecto.rs project.
- [timescale/pgai](https://github.com/timescale/pgai): PostgreSQL extension to allow RAG, semantic search and other AI application development from within postgres. Based on pgvector.
- [timescale/pgvectorscale](https://github.com/timescale/pgvectorscale): DiskANN vector index implementation complementary to pgvector.

### Hybrid

- [plpgsql_bm25rrf.sql](https://github.com/jankovicsandras/plpgsql_bm25): Hybrid search (BM25+pgvector) with Reciprocal Rank Fusion implemented in PL/pgSQL

## Time Series

- [timescale/timescaledb](https://github.com/timescale/timescaledb): TimescaleDB is PostgreSQL++ for time series and events.
- [tembo-io/pg_timeseries](https://github.com/tembo-io/pg_timeseries): Open-source time-series extension for PostgreSQL

## Column Oriented

- [paradedb/paradedb](https://github.com/paradedb/paradedb): Postgres for Search and Analytics
- [hydradatabase/hydra](https://github.com/hydradatabase/hydra)
- [citusdata/cstore_fdw](https://github.com/citusdata/cstore_fdw)
- [pg_duckdb](https://github.com/duckdb/pg_duckdb): DuckDB column storage inside Postgres

## NoSQL

- [JSON Types](https://www.postgresql.org/docs/current/datatype-json.html): Native support for JSON support in PostgreSQL
- [robconery/dox](https://github.com/robconery/dox)
- https://www.ferretdb.com
- [Using JSONB in PostgreSQL®: How to Effectively Store & Index JSON Data in PostgreSQL](https://scalegrid.io/blog/using-jsonb-in-postgresql-how-to-effectively-store-index-json-data-in-postgresql/)

## Graph Data

- [Apache Age](https://age.apache.org): Graph Database for PostgreSQL to provide graph data processing and analytics capability to all relational databases.

## Foreign Data

- [supabase/wrappers](https://github.com/supabase/wrappers)

## HTTP

- [pramsey/pgsql-http](https://github.com/pramsey/pgsql-http)
- [supabase/pg_net](https://github.com/supabase/pg_net)

## API Platforms

- [PostgREST](https://github.com/PostgREST/postgrest): RESTful API from any existing PostgreSQL database
- [Hasura GraphQL Engine](https://github.com/hasura/graphql-engine): Metadata-driven API platform

## GraphQL and Alternative Query Languages

- [PostGraphile](https://postgraphile.org): Extensible high-performance automatic GraphQL API for PostgresSQL
- [supabase/pg_graphql](https://supabase.github.io/pg_graphql): PostgreSQL extension that enables querying the database with GraphQL using a single SQL function
- [dosco/graphjin](https://github.com/dosco/graphjin): GraphJin automatically converts GraphQL into SQL queries
- [kaspermarstal/plprql](https://github.com/kaspermarstal/plprql): PostgreSQL extension to write functions using [PRQL](https://prql-lang.org/) (Pipelined Relational Query Language)

## Events, Replication, CDC

- [aws/pgactive](https://github.com/aws/pgactive): Replication extension for creating an active-active database by AWS.
- [xataio/pgstream](https://github.com/xataio/pgstream): CDC command-line tool and library that offers Postgres replication support with DDL changes to any provided output.
- [electric-sql/electric](https://github.com/electric-sql/electric): HTTP API that enables synching [Shapes](https://electric-sql.com/docs/guides/shapes) (i.e. segments) of a Postgres database. It's like GraphQL for Postgres databases.
- [The Notifier Pattern for Applications That Use Postgres](https://brandur.org/notifier)
- [SQL Notify](https://www.postgresql.org/docs/current/sql-notify.html)
- [cpursley/walex](https://github.com/cpursley/walex) (Disclosure: I maintain this and think it's pretty awesome)
- [PeerDB-io/peerdb](https://github.com/PeerDB-io/peerdb)
- [debezium/debezium](https://github.com/debezium/debezium)
- [2ndQuadrant/pglogical](https://github.com/2ndQuadrant/pglogical)

## Caching

- [tidwall/pogocache](https://github.com/tidwall/pogocache?tab=readme-ov-file#postgres): caching layer with a focus on latency and CPU efficiency.
- https://martinheinz.dev/blog/105
- [readysettech/readyset](https://github.com/readysettech/readyset)

## Unit Tests

- [theory/pgtap](https://github.com/theory/pgtap)
- [peterldowns/pgtestdb](https://github.com/peterldowns/pgtestdb)

## HTML & Applications

- [SQLpage](https://github.com/lovasoa/SQLpage)
- [Omnigres](https://github.com/omnigres/omnigres)
- [pg_render](https://github.com/mkaski/pg_render)
- [plmustache](https://github.com/PostgREST/plmustache)

## Migrations

- [purcell/postgresql-migrations](https://github.com/purcell/postgresql-migrations)
- [www.bytebase.com/](https://www.bytebase.com/)
- [xataio/pgroll](https://github.com/xataio/pgroll)
- [stripe/pg-schema-diff](https://github.com/stripe/pg-schema-diff)
- [pgschema/pgschema](https://github.com/pgschema/pgschema): CLI tool that brings terraform-style declarative schema migration workflow to Postgres.

## Performance Tuning

- [Supabase Index Advisor](https://github.com/supabase/index_advisor)
- [Dexter](https://github.com/ankane/dexter)
- [HypoPG](https://github.com/HypoPG/hypopg)
- [pg_hint_plan](https://github.com/ossc-db/pg_hint_plan)
- [PGHero](https://github.com/ankane/pghero)
- [pg_incremental](https://github.com/CrunchyData/pg_incremental): Extension to do fast, reliable, incremental batch processing.
- [pgassistant](https://github.com/beh74/pgassistant-community): PostgreSQL assistant for developers designed to help understand and optimize PostgreSQL database performance

## Monitoring

- [StatsMgr](https://codeberg.org/Data-Bene/StatsMgr): Efficient and organized management of statistics across WAL, SLRU, checkpointing, & more. Currently supports dynamic initialization, shared memory utilization, and SQL interfaces.
- [pgMonitor](https://github.com/CrunchyData/pgmonitor): A monitoring solution that visualizes metrics using Prometheus, Grafana, SQL Exporter, and the pgMonitor extension.

## Scaling & Storage

- [How Cloudflare Achieved 55 Million Requests per Second with Just 15 PostgreSQL Clusters!](https://levelup.gitconnected.com/how-cloudflare-achieved-55-million-requests-per-second-with-just-15-postgresql-clusters-2d8a28ffd100)
- [supabase/supavisor](https://github.com/supabase/supavisor)
- [pg-sharding/spqr](https://github.com/pg-sharding/spqr)
- [pgdogdev/pgdog](https://github.com/pgdogdev/pgdog): PgDog is a transaction pooler and logical replication manager that can shard PostgreSQL. Written in Rust, PgDog is fast, secure and can manage hundreds of databases and hundreds of thousands of connections.
- [orioledb.com/](https://www.orioledb.com): OrioleDB is a PostgreSQL extension that combines the advantages of both on-disk and in-memory engines. It uses PostgreSQL pluggable storage to increase performance and cut costs.

## User Interfaces & Dashboards

- [Baserow](https://baserow.io)
- [NocoDB](https://github.com/nocodb/nocodb)
- [AppSmith](https://appsmith.com)
- [mathesar-foundation/mathesar](https://github.com/mathesar-foundation/mathesar): Intuitive spreadsheet-like interface that lets users of all technical skill levels view, edit, query, and collaborate on Postgres data directly—self hosted, with native Postgres access control.

## Visualization

### Graphics Visualization

- [dr-jts/pg_svg](https://github.com/dr-jts/pg_svg): Collection of PostgreSQL functions to create SVG graphics intended to convert PostGIS geometries into styled SVG documents

### Data Visualization

- [Evidence](https://evidence.dev)
- [Metabase](https://metabase.com)
- [Hopara](https://hopara.io): Platform for real-time data visualization intended for Manufacturing, IoT, Life Science and Data Lakes.

## Package Management

- [pgxman/pgxman](https://github.com/pgxman/pgxman)
- [supabase/dbdev](https://github.com/supabase/dbdev)

## Language Servers

- [supabase/postgres-language-server](https://github.com/supabase-community/postgres-language-server): A collection of language tools and a Language Server Protocol (LSP) implementation for Postgres, focusing on developer experience and reliable SQL tooling.

## Data Privacy & Security (or Data Masking)

- [neondatabase/postgresql_anonymizer](https://github.com/neondatabase/postgresql_anonymizer): A PostgreSQL extension to directly mask or replace Personally Identifiable Information (PII) or commercially sensitive data.

## Financial Ledgers

- [pgledger](https://github.com/pgr0ss/pgledger): A double entry ledger implementation in PostgreSQL 

## Miscellaneous

- [Very comprehensive list of Postgres tooling](https://gist.github.com/mjf/d885e3631c3eaa8a5a9ea62c5c20407c)
- [Unsupported PostgreSQL features in Aurora DSQL](https://docs.aws.amazon.com/aurora-dsql/latest/userguide/working-with-postgresql-compatibility-unsupported-features.html): AWS has a new database engine called Aurora DSQL, and explicitly listed what PostgreSQL features are not supported.
