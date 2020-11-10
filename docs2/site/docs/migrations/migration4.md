# Migrating from v3.x to v4.x

## New Features

## Breaking Changes

* `NameConverter` and `SchemaFilter` have been removed from `ExecutionOptions` and are now properties on the `Schema`.

* `GraphQL.Utilities.ServiceProviderExtensions` has been made internal. This affects usages of its extension method `GetRequiredService`. Instead, reference the `Microsoft.Extensions.DependencyInjection.Abstractions` NuGet package and use the extension method provided by the `Microsoft.Extensions.DependencyInjection.ServiceProviderServiceExtensions` class.

* New property `GraphQL.Introspection.ISchemaComparer ISchema.Comparer { get; set; }`
