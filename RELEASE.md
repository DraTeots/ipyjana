- To release a new version of ipyjana on PyPI:

Update _version.py (set release version, remove 'dev')
git add the _version.py file and git commit
```bash
python setup.py sdist upload
python setup.py bdist_wheel upload
```

  ```bash
  python setup.py sdist bdist_wheel
  ```

  ```bash
  
  twine upload dist/ipyjana*
  ```
  
- To release a new version of ipyjana on NPM:

```
# clean out the `dist` and `node_modules` directories
git clean -fdx
npm install
npm publish
```