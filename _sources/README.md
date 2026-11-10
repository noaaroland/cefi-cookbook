[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://noaa-cefi-portal.github.io/cefi-cookbook/content/cefi_goal.html)
# NOAA Changing, Ecosystems, and Fisheries Initiative (CEFI) Data Cookbook

## How to Use the CEFI Cookbook ?
The CEFI Cookbook aims to provide valuable information to users of varying expertise levels. We encourage users to navigate directly to specific topics and pages as needed. Our goal is to make each topic and page self-contained, providing links to associated resources when prior knowledge is required. A quick breakdown of the resources provided is shown below

## What resources are provided
- Introduction to CEFI
- Introduction to regional MOM6
- Computational environment setup for CEFI analyses
- Tutorials on accessing CEFI related data
- Derivation of marine resource related indexes
- Free and light cloud computation

You need to activate the environment you used to install the build tools. For example if you used a virtual environment called .vene use:
```
source .venv/bin/activate
```
N.B. For some changes, jupyter-book will not be aware that the structure has changed. It has no internal tracking
mechanism. Therefore, before publishing, it's a good idea to build the entire book from scratch to make sure all the
changes are applied.

To clean:
 ```
jupyter-book clean .
```

To build:
```
jupyter-book build .
```

To publish on github pages:
```
ghp-import -n -p -f _build/html
```

To view locally with a server (use the port of your choice):
```
cd _build/html
python -m http.server 8080
```
and open
http://localhost:8080/
in your browser.