# Project structure

The framework codebase is split into a number of submodules, making it possible to only use what is needed.

* **Core**
  * **Revo.Core** Implements framework’s core features like events or commands and defines basic struc-tures and interfaces for things like the unit of work pattern, security permissions and other utilities.
  * **Revo.DataAccess** Lower-level data access layer that provides interfaces and other abstractions for working with databases, independent of domain concepts \(aggregates, consistency boundaries, etc.\).
  * **Revo.Domain** Defines most of the framework’s building blocks for an application domain model – i.e. aggregates, entities, sagas, etc.
  * **Revo.Infrastructure** Interfaces for working with application domain and related aspects of an applications – e.g. aggregate repositories, event stores, projections, jobs, asynchronous event queues, etc.
  * **Revo.Testing** Provides several useful facilities for easier application testing – e.g. assertions for event-sourced aggregates or fake repositories \(refer to the [Testing](../../reference-guide/testing.md) chapter\).
* **Providers**
  * **Revo.AspNetCore** Provides support for ASP.NET applications – application life cycle hooks, user context, authentication, etc.
  * **Revo.AspNet** Provides support for ASP.NET applications – application life cycle hooks, user context, authentication, etc.
  * **Revo.EFCore**
  * **Revo.EF6**
  * **Revo.Hangfire** Hangfire integration for background jobs.
  * **Revo.Raven** Data access layer implementation using RavenDB database system.
  * **Revo.Rebus** Rebus integration for command/query and event messaging with RabbitMQ.
* **Tests**
* **Examples**
