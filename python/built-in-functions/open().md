# open()

```python
"""
with w option, new file will be created if the target file is not existed.
If target file is existed, contents will be overwritten(former contents will deleted).
"""
f = open('file_name.txt', 'w')

"""
with w option, new file will be created if the target file is not existed.
If target file is existed, contents will be added so former contents will not be deleted.
"""
f = open('file_name.txt', 'a')

"""
with w option, new file will be created if the target file is not existed.
If target file is existed, FileExistsError is occurred.
"""
f = open('file_name.txt', 'x')

```
