# RESTful Resource Naming Conventions

## CRUD on a resource

- Get a user with id `id` should be GET: `/users/{id}`
- Create a new user should be POST: `/users`
- Update a user should be PUT: `/users/{id}` with body as the whole use model data.
- Partially update a user resouce should be PATCH: `/users/{id}`

## URIs as resources as nouns

The end-point should take the form of a noun instead of verb.


For example: we should use `/users/{id}` instead of `/getUser`

## Pluralized resources

This is a matter of preference; however, most API design experts would suggest you pluralize all resources unless they are singleton resources.

Example: `/users` (typical resource) or `/users/{id}/address` (singleton resource)

## Forward slashes for hierarchy

As shown in the examples above, forward slashes are conventionally used to show the hierarchy between individual resources and collections.

Example: `/users/{id}/address` clearly falls under the `/users/{id}` resource which falls under the `/users` collection.


## Lowercase letters and dashes
By convention, resource names should use exclusively lowercase letters. Similarly, dashes (-) are conventionally used in place of underscores (_).

Example: `/users/{id}/pending-orders` instead of `/users/{id}/Pending_Orders`



