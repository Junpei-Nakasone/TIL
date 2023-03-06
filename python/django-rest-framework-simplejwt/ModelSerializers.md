Using ModelSerializer, you can define serializer by specifying model and fields.

models.py
```python
class Snippet(models.Model):
    created = models.DateTimeField(auto_now_add=True)
    title = models.CharField(max_length=100, blank=True, default='')
```

serializers.py
```python
class SnippetSerializer(serializers.ModelSerializer):
    class Meta:
        model = Snippet
        fields = ['id', 'title']
```

`ModelSerializer` classes don't do anything magical, they are simply a shortcut for creating serializer classes:
- An automatically determined set of fields.
- Simple default implementations  for the `create()` and `update()` methods.
