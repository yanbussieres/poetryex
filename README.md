### ISSUE

`brew install poetry` requires `python@3.9` which automatically installed `pip 20.2.3`
- Run `poetry install` from main will fail, with the following error message : 
```
File "/private/var/folders/5d/yl0b7h4x00s0jt_zjqy58r040000gn/T/pip-build-env-9wozdm6g/overlay/lib/python3.9/site-packages/poetry/core/packages/directory_dependency.py", line 36, in __init__
          raise ValueError("Directory {} does not exist".format(self._path))
      ValueError: Directory ../dep1 does not exist
```
#### Solution (kind of)

- Get an earlier version of poetry installed locally through `brew`. (but you have to do it locally since there is only one formula for installing poetry with brew)

**OR**

-  Keep the same setup, downgrade pip to <19. 
