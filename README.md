# Setting up & testing RTD on Alibaba Cloud ECS

## Chinese PDF support
Add the following code to conf.py

```python
# -- Options for PDF output -------------------------------------------------

# use xelatex to override original latex engine for CN support
latex_engine = 'xelatex'
latex_use_xindy = False
latex_elements = {
    'preamble': '\\usepackage[UTF8]{ctex}\n',
}
```

## Use RTD sphinx theme
Install theme on server
```python
$ pip install sphinx-rtd-theme
```

Add the following code to conf.py

```python
import sphinx_rtd_theme

extensions = [
    ...
    "sphinx_rtd_theme",
]

html_theme = "sphinx_rtd_theme"
```
