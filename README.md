# mkdocs-material
docker image of the awesome squidfunk/mkdocs-material with some extensions added

## fix memo

```
#6 16.29         output = pypandoc.convert(markdown_filename, 'rst', format='md')
#6 16.29     AttributeError: module 'pypandoc' has no attribute 'convert'
#6 16.29     ----------------------------------------
```

> In the recent release of PyPandoc (version 1.8), the convert function was removed after a year of being deprecated.
https://github.com/man-group/pytest-plugins/issues/87#issuecomment-1123830409

here

https://github.com/msabramo/setuptools-markdown/blob/master/setuptools_markdown.py#L43

https://github.com/msabramo/setuptools-markdown/pull/21
