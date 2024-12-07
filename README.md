# Postgres for Everything (e/postgres)<!-- omit in toc -->

Keep It Simple Stupid, just use postgres.

## Goals & Inspiration <!-- omit in toc -->

The goal of this repository is to demonstrate how to use **Postgres for Everything**.

It's inspired by [this article](https://www.amazingcto.com/postgres-for-everything/)
from the [Amazing CTO](https://www.amazingcto.com/) as well as
[this GitHub gist](https://gist.github.com/cpursley/c8fb81fe8a7e5df038158bdfe0f06dbb)
from [@cpursley](https://gist.github.com/cpursley).

## Why maintain this list? <!-- omit in toc -->

It seems like every week I hear of a new tool on top of Postgres or another way
it can being used, so I wanted a place where I can keep track of everything. If
you have other examples, [submit a PR](<[Olshansk/postgres_for_everything](https://github.com/Olshansk/postgres_for_everything)/pulls>)!

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
- [Scaling \& Storage](#scaling--storage)
- [Dashboards \& UIs](#dashboards--uis)
- [Data Visualization](#data-visualization)
- [Package Management](#package-management)
- [Language Servers](#language-servers)
- [Miscellaneous](#miscellaneous)
- [Bonus: How many items include Supabase?](#bonus-how-many-items-include-supabase)

## Blog Posts & Articles

- [Simplify: move code into database functions](https://sive.rs/pg)
- [Just Use Postgres for Everything](https://www.amazingcto.com/postgres-for-everything/)
- [PostgreSQL is the worlds’ best database](https://www.2ndquadrant.com/en/blog/postgresql-is-the-worlds-best-database/)
- [Postgres is eating the database world](https://medium.com/@fengruohang/postgres-is-eating-the-database-world-157c204dcfc4)
- [Hacker News discussion](https://news.ycombinator.com/item?id=39273954)

## Cron Jobs

- [citusdata/pg_cron]([citusdata/pg_cron)](https://github.com/citusdata/pg_cron))
- [cybertec-postgresql/pg_timetable]([cybertec-postgresql/pg_timetable)](https://github.com/cybertec-postgresql/pg_timetable))

## Message Queues

- https://adriano.fyi/posts/2023-09-24-choose-postgres-queue-technology
- [tembo-io/pgmq](https://github.com/tembo-io/pgmq)
- [SKIP LOCKED](https://www.2ndquadrant.com/en/blog/what-is-select-skip-locked-for-in-postgresql-9-5/)
- [riverqueue/river](https://github.com/riverqueue/river)
- [sequinstream/sequin](https://github.com/sequinstream/sequin): Sequin is a tool for change data capture (CDC) in Postgres. Sequin makes it easy to stream Postgres rows and changes to streaming platforms and queues (e.g. Kafka and SQS). You can backfill existing rows and stream new changes in real-time.

## Analytics

- [pg_analytics: Transforming Postgres into a Fast OLAP Database](https://blog.paradedb.com/pages/introducing_analytics)

## GIS & Mapping

- [postgis/postgis](https://github.com/postgis/postgis)

## Audit Logs

- [arkhipov/temporal_tables](https://github.com/arkhipov/temporal_tables)
- [supabase/supa_audit](https://github.com/supabase/supa_audit)
- [pgMemento/pgMemento](https://github.com/pgMemento/pgMemento)
- [pgaudit/pgaudit](https://github.com/pgaudit/pgaudit)

## Access Control & Authorization

- [arkhipov/acl](https://github.com/arkhipov/acl)
- https://www.postgresql.org/docs/current/pgcrypto.html
- [michelp/pgjwt](https://github.com/michelp/pgjwt)
- [supabase.com/docs/guides/database/vault](https://supabase.com/docs/guides/database/vault))

## Search

### Full Text

- [Postgres Full Text Search](https://gist.github.com/cpursley/e3586382c3a42c54ca7f5fef1665be7b) (bunch of helpful links)
- [paradedb/paradedb](https://github.com/paradedb/paradedb)
- [Postgres Full Text Search vs the rest](https://supabase.com/blog/postgres-full-text-search-vs-the-rest)

### Vector

- [neondatabase/pg_embedding](https://github.com/neondatabase/pg_embedding)
- [pgvector/pgvector](https://github.com/pgvector/pgvector)
- [tensorchord/VectorChord](https://github.com/tensorchord/VectorChord): PostgreSQL extension designed for scalable, high-performance, and disk-efficient vector similarity search. It serves as the successor to the pgvecto.rs project.

## Time Series

- [timescale/timescaledb](https://github.com/timescale/timescaledb)
- [tembo-io/pg_timeseries](https://github.com/tembo-io/pg_timeseries)
  - [Introducing pg_timeseries: Open-source time-series extension for PostgreSQL](https://tembo.io/blog/pg-timeseries)

## Column Oriented

- [hydradatabase/hydra](https://github.com/hydradatabase/hydra)
- [citusdata/cstore_fdw](https://github.com/citusdata/cstore_fdw)

## NoSQL

- https://www.postgresql.org/docs/current/datatype-json.html
- [robconery/dox](https://github.com/robconery/dox)
- https://www.ferretdb.com
- [Using JSONB in PostgreSQL®: How to Effectively Store & Index JSON Data in PostgreSQL](https://scalegrid.io/blog/using-jsonb-in-postgresql-how-to-effectively-store-index-json-data-in-postgresql/)

## Graph Data

- https://age.apache.org

## Foreign Data

- [supabase/wrappers](https://github.com/supabase/wrappers)

## Alternative Query Languages

- [kaspermarstal/plprql](https://github.com/kaspermarstal/plprql)
- [supabase.github.io/pg_graphql](https://supabase.github.io/pg_graphql)
- [dosco/graphjin](https://github.com/dosco/graphjin)

## HTTP

- [pramsey/pgsql-http](https://github.com/pramsey/pgsql-http)
- [supabase/pg_net](https://github.com/supabase/pg_net)

## APIs

- [PostgREST/postgrest](https://github.com/PostgREST/postgrest)
- [hasura/graphql-engine](https://github.com/hasura/graphql-engine)
- [postgraphile.org](https://postgraphile.org)
- [supabase.github.io/pg_graphql](https://supabase.github.io/pg_graphql)

## Events, Replication, CDC

- [The Notifier Pattern for Applications That Use Postgres](https://brandur.org/notifier)
- https://www.postgresql.org/docs/current/sql-notify.html
- [cpursley/walex (Disclosure: I maintain this and think it's pretty awesome)](https://github.com/cpursley/walex "Disclosure: I maintain this and think it's pretty awesome")
- [PeerDB-io/peerdb](https://github.com/PeerDB-io/peerdb)
- [debezium/debezium](https://github.com/debezium/debezium)
- [2ndQuadrant/pglogical](https://github.com/2ndQuadrant/pglogical)

## Caching

- https://martinheinz.dev/blog/105
- [readysettech/readyset](https://github.com/readysettech/readyset)

## Unit Tests

- [theory/pgtap](https://github.com/theory/pgtap)
- [peterldowns/pgtestdb](https://github.com/peterldowns/pgtestdb)

## HTML & Applications

- [SQLpage]([lovasoa/SQLpage)](https://github.com/lovasoa/SQLpage))
- [Omnigres]([omnigres/omnigres)](https://github.com/omnigres/omnigres))
- [pg_render]([mkaski/pg_render)](https://github.com/mkaski/pg_render))
- [plmustache]([PostgREST/plmustache)](https://github.com/PostgREST/plmustache))

## Graphics & Visualizations

- [pgSVG]([dr-jts/pg_svg)](https://github.com/dr-jts/pg_svg))

## Migrations

- [purcell/postgresql-migrations](https://github.com/purcell/postgresql-migrations)
- [www.bytebase.com/](https://www.bytebase.com/)
- [xataio/pgroll](https://github.com/xataio/pgroll)
- [stripe/pg-schema-diff](https://github.com/stripe/pg-schema-diff)

## Performance Tuning

- [Supabase Index Advisor]([supabase/index_advisor)](https://github.com/supabase/index_advisor))
- [Dexter]([ankane/dexter)](https://github.com/ankane/dexter))
- [HypoPG]([HypoPG/hypopg)](https://github.com/HypoPG/hypopg))
- [pg_hint_plan]([ossc-db/pg_hint_plan)](https://github.com/ossc-db/pg_hint_plan))
- [PGHero]([ankane/pghero)](https://github.com/ankane/pghero))

## Scaling & Storage

- [How Cloudflare Achieved 55 Million Requests per Second with Just 15 PostgreSQL Clusters!](https://levelup.gitconnected.com/how-cloudflare-achieved-55-million-requests-per-second-with-just-15-postgresql-clusters-2d8a28ffd100)
- [supabase/supavisor](https://github.com/supabase/supavisor)
- [pg-sharding/spqr](https://github.com/pg-sharding/spqr)
- [orioledb.com/](https://www.orioledb.com): OrioleDB is a PostgreSQL extension that combines the advantages of both on-disk and in-memory engines. It uses PostgreSQL pluggable storage to increase performance and cut costs.

## Dashboards & UIs

- [Baserow](https://baserow.io)
- [NocoDB]([nocodb/nocodb)](https://github.com/nocodb/nocodb))
- [AppSmith](https://appsmith.com)

## Data Visualization

- [Evidence](https://evidence.dev)
- [Metabase](https://metabase.com)

## Package Management

- [pgxman/pgxman](https://github.com/pgxman/pgxman)
- [supabase/dbdev](https://github.com/supabase/dbdev)

## Language Servers

- [supabase/postgres_lsp](https://github.com/supabase/postgres_lsp)

## Miscellaneous

- [Very comprehensive list of Postgres tooling](https://gist.github.com/mjf/d885e3631c3eaa8a5a9ea62c5c20407c)
- [Unsupported PostgreSQL features in Aurora DSQL](https://docs.aws.amazon.com/aurora-dsql/latest/userguide/working-with-postgresql-compatibility-unsupported-features.html): AWS has a new database engine called Aurora DSQL, and explicitly listed what PostgreSQL features are not supported.

## Bonus: How many items include Supabase?

11
