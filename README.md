# Postgres for Everything <!-- omit in toc -->

Keep it simple, use Postgres for everything.

## Goals & Inspiration <!-- omit in toc -->

The goal of this repository is to demonstrate how to use **Postgres for Everything**.

It's inspired by [this article](https://www.amazingcto.com/postgres-for-everything/)
from the [Amazing CTO](https://www.amazingcto.com/) as well as
[this GitHub gist](https://gist.github.com/cpursley/c8fb81fe8a7e5df038158bdfe0f06dbb)
from [@cpursley](https://gist.github.com/cpursley).

It seems like every week I hear of a new tool on top of Postgres or another way
it can being used, so I wanted a place where I can keep track of everything. If
you have other examples, [submit a PR](https://github.com/Olshansk/postgres_for_everything/pulls)!

## Table of Contents <!-- omit in toc -->

- [Blog Posts \& Articles](#blog-posts--articles)
- [Cron Jobs](#cron-jobs)
- [Message Queues](#message-queues)
- [Analytics](#analytics)
- [GIS \& Mapping](#gis--mapping)
- [Audit Logs](#audit-logs)
- [Access Control \& Authorization](#access-control--authorization)
- [Search](#search)
  - [Full Text](#full-text)
  - [Vector](#vector)
- [Time Series](#time-series)
- [Column Oriented](#column-oriented)
- [NoSQL](#nosql)
- [Graph Data](#graph-data)
- [Foreign Data](#foreign-data)
- [Alternative Query Languages](#alternative-query-languages)
- [HTTP](#http)
- [APIs](#apis)
- [Events, Replication, CDC](#events-replication-cdc)
- [Caching](#caching)
- [Unit Tests](#unit-tests)
- [HTML \& Applications](#html--applications)
- [Graphics \& Visualizations](#graphics--visualizations)
- [Migrations](#migrations)
- [Performance Tuning](#performance-tuning)
- [Scaling](#scaling)
- [Dashboards \& UIs](#dashboards--uis)
- [Data Visualization](#data-visualization)
- [Package Management](#package-management)
- [Language Servers](#language-servers)
- [Miscellaneous](#miscellaneous)

## Blog Posts & Articles

- [Simplify: move code into database functions](https://sive.rs/pg)
- [Just Use Postgres for Everything](https://www.amazingcto.com/postgres-for-everything/)
- [PostgreSQL is the worlds’ best database](https://www.2ndquadrant.com/en/blog/postgresql-is-the-worlds-best-database/)
- [Postgres is eating the database world](https://medium.com/@fengruohang/postgres-is-eating-the-database-world-157c204dcfc4)
- [Hacker News discussion](https://news.ycombinator.com/item?id=39273954)

## Cron Jobs

- https://github.com/citusdata/pg_cron
- https://github.com/cybertec-postgresql/pg_timetable

## Message Queues

- https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology
- https://github.com/tembo-io/pgmq
- [SKIP LOCKED](https://www.2ndquadrant.com/en/blog/what-is-select-skip-locked-for-in-postgresql-9-5/)
- https://github.com/riverqueue/river

## Analytics

- [pg_analytics: Transforming Postgres into a Fast OLAP Database](https://blog.paradedb.com/pages/introducing_analytics)

## GIS & Mapping

- https://github.com/postgis/postgis

## Audit Logs

- https://github.com/arkhipov/temporal_tables
- https://github.com/supabase/supa_audit
- https://github.com/pgMemento/pgMemento
- https://github.com/pgaudit/pgaudit

## Access Control & Authorization

- https://github.com/arkhipov/acl
- https://www.postgresql.org/docs/current/pgcrypto.html
- https://github.com/michelp/pgjwt
- https://supabase.com/docs/guides/database/vault

## Search

### Full Text

- [Postgres Full Text Search](https://gist.github.com/cpursley/e3586382c3a42c54ca7f5fef1665be7b) (bunch of helpful links)
- https://github.com/paradedb/paradedb
- [Postgres Full Text Search vs the rest](https://supabase.com/blog/postgres-full-text-search-vs-the-rest)

### Vector

- https://github.com/neondatabase/pg_embedding
- https://github.com/pgvector/pgvector

## Time Series

- https://github.com/timescale/timescaledb
- https://github.com/tembo-io/pg_timeseries
  - [Introducing pg_timeseries: Open-source time-series extension for PostgreSQL](https://tembo.io/blog/pg-timeseries)

## Column Oriented

- https://github.com/hydradatabase/hydra
- https://github.com/citusdata/cstore_fdw

## NoSQL

- https://www.postgresql.org/docs/current/datatype-json.html
- https://github.com/robconery/dox
- https://www.ferretdb.com
- [Using JSONB in PostgreSQL®: How to Effectively Store & Index JSON Data in PostgreSQL](https://scalegrid.io/blog/using-jsonb-in-postgresql-how-to-effectively-store-index-json-data-in-postgresql/)

## Graph Data

- https://age.apache.org

## Foreign Data

- https://github.com/supabase/wrappers

## Alternative Query Languages

- https://github.com/kaspermarstal/plprql
- https://supabase.github.io/pg_graphql
- https://github.com/dosco/graphjin

## HTTP

- https://github.com/pramsey/pgsql-http
- https://github.com/supabase/pg_net

## APIs

- https://github.com/PostgREST/postgrest
- https://github.com/hasura/graphql-engine
- https://postgraphile.org
- https://supabase.github.io/pg_graphql

## Events, Replication, CDC

- [The Notifier Pattern for Applications That Use Postgres](https://brandur.org/notifier)
- https://www.postgresql.org/docs/current/sql-notify.html
- https://github.com/cpursley/walex (Disclosure: I maintain this and think it's pretty awesome)
- https://github.com/PeerDB-io/peerdb
- https://github.com/debezium/debezium
- https://github.com/2ndQuadrant/pglogical

## Caching

- https://martinheinz.dev/blog/105
- https://github.com/readysettech/readyset

## Unit Tests

- https://github.com/theory/pgtap
- https://github.com/peterldowns/pgtestdb

## HTML & Applications

- [SQLpage](https://github.com/lovasoa/SQLpage)
- [Omnigres](https://github.com/omnigres/omnigres)
- [pg_render](https://github.com/mkaski/pg_render)
- [plmustache](https://github.com/PostgREST/plmustache)

## Graphics & Visualizations

- [pgSVG](https://github.com/dr-jts/pg_svg)

## Migrations

- https://github.com/purcell/postgresql-migrations
- https://www.bytebase.com/
- https://github.com/xataio/pgroll
- https://github.com/stripe/pg-schema-diff

## Performance Tuning

- [Index Advisor](https://github.com/supabase/index_advisor)
- [Dexter](https://github.com/ankane/dexter)
- [HypoPG](https://github.com/HypoPG/hypopg)
- [pg_hint_plan](https://github.com/ossc-db/pg_hint_plan)
- [PGHero](https://github.com/ankane/pghero)

## Scaling

- [How Cloudflare Achieved 55 Million Requests per Second with Just 15 PostgreSQL Clusters!](https://levelup.gitconnected.com/how-cloudflare-achieved-55-million-requests-per-second-with-just-15-postgresql-clusters-2d8a28ffd100)
- https://github.com/supabase/supavisor
- https://github.com/pg-sharding/spqr

## Dashboards & UIs

- [Baserow](https://baserow.io)
- [NocoDB](https://github.com/nocodb/nocodb)
- [AppSmith](https://appsmith.com)

## Data Visualization

- [Evidence](https://evidence.dev)
- [Metabase](https://metabase.com)

## Package Management

- https://github.com/pgxman/pgxman
- https://github.com/supabase/dbdev

## Language Servers

- https://github.com/supabase/postgres_lsp

## Miscellaneous

- [Very comprehensive list of Postgres tooling](https://gist.github.com/mjf/d885e3631c3eaa8a5a9ea62c5c20407c)
