# Setting up & testing RTD on Alibaba Cloud ECS

## Chinese PDF support
Add the following code to conf.py

```
# -- Options for PDF output -------------------------------------------------

# use xelatex to override original latex engine for CN support
latex_engine = 'xelatex'
latex_use_xindy = False
latex_elements = {
    'preamble': '\\usepackage[UTF8]{ctex}\n',
}
```
