### ViewSets
Django REST framework allows you to combine the logic for a set of related views in a single class, called `ViewSet`. In other frameworks you may also find conceptually similar implementations named something like "Resources" or "Controllers".
A `ViewSet` class is simply a type of class-based View, that does not provide any method handlers such as `.get()` or `.post()`, and instead provides actions such as `.list()` and `.create()`.
The method handlers for `ViewSet` are only bound to the corresponding actions at the point of finalizing the view, using the `.as_view()` method.
