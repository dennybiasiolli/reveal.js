#### 🫣 Circular dependencies

<small>

> To manually resolve a CircularDependencyError, break out one of the ForeignKeys in the circular dependency loop into a separate migration, and move the dependency on the other app with it.
> 
> If you’re unsure, see how makemigrations deals with the problem when asked to create brand new migrations from your models. In a future release of Django, squashmigrations will be updated to attempt to resolve these errors itself.

https://docs.djangoproject.com/en/4.1/topics/migrations/#squashing-migrations

</small>


<aside class="notes">
</aside>
