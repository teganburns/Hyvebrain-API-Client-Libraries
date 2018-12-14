
### Note To Self:

Change Dir:
```
cd $gitpath/Hyvebrain-API-Client-Libraries/src/python/Hyvebrain/
```

Build the package:
```
python3 setup.py sdist bdist_wheel
```

Upload to test:
```
twine upload --skip-existing  --repository-url https://test.pypi.org/legacy/ dist/*
```

Install test:
```
python -m pip install --user -i https://test.pypi.org/simple/ hyvebrain --upgrade
```

Run Tests:
```
python -m pip show hyvebrain
```

Uninstall Tests:
```
python -m pip uninstall hyvebrain
```

Upload to official:
```
twine upload --skip-existing dist/*
```

Install official:
```
python -m pip install --user hyvebrain --upgrade
```

