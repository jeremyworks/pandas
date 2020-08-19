# jeremyworks/pandas
This codebase helps answer some of there questions:
* **_How do I quickly load data from a URL?_**  
* **_What does my JSON or XML data look like?_**  
* **_What are the fields and data ranges?_**  
* **_How complete is the data?_**  


This repository includes [Jupyter](https://jupyter.org/) notebooks, samples, and resources for processing data in [pandas](https://pandas.pydata.org/docs/).
Code samples can easily be run if you have [Docker](https://www.docker.com/) installed or through Binder.


# Binder (no docker)
Binder allows you to run jupyter notebooks through a URL is the source code for the notebook is
publicly visible on github. This is a great way to quickly check out notebooks and run quick
commands, but you _can't actually save any changes_ and the resources might be limited.

* Parsing JSON data from URL - [JSON from URL Binder Link](https://mybinder.org/v2/gh/jeremyworks/pandas/master?filepath=json%2FJson-URL-to-Pandas.ipynb)
* Parsing JSON w/caching - [JSON w/caching Binder Link](https://mybinder.org/v2/gh/jeremyworks/pandas/master?filepath=json%2FJson-to-Pandas.ipynb)

# Local Docker 
## Parsing JSON
Pull data in JSON format into pandas DataFrames for analysis.

```bash
git clone git@github.com:jeremyworks/pandas.git
``` 

Start a local jupyter notebook and expose it in a browser on port 8888.
```bash
cd pandas
docker run -p 8888:8888 -v `pwd`/json:/home/jovyan/work jeremyworks/jupyter-scipy:1.0.0
```

The output will look something like this below. Follow the link specified with the unique token output in the console-  
http://127.0.0.1:8888/?token=..........

```text
Executing the command: jupyter notebook
[I 20:31:05.107 NotebookApp] Writing notebook server cookie secret to /home/jovyan/.local/share/jupyter/runtime/notebook_cookie_secret
[I 20:31:06.640 NotebookApp] JupyterLab extension loaded from /opt/conda/lib/python3.7/site-packages/jupyterlab
[I 20:31:06.640 NotebookApp] JupyterLab application directory is /opt/conda/share/jupyter/lab
[I 20:31:06.644 NotebookApp] Serving notebooks from local directory: /home/jovyan
[I 20:31:06.644 NotebookApp] The Jupyter Notebook is running at:
[I 20:31:06.645 NotebookApp] http://1b1bb1843ab0:8888/?token=70fd77edc3cf5b63cb3dccbceb172edec613882bca141feb
[I 20:31:06.645 NotebookApp]  or http://127.0.0.1:8888/?token=70fd77edc3cf5b63cb3dccbceb172edec613882bca141feb
[I 20:31:06.645 NotebookApp] Use Control-C to stop this server and shut down all kernels (twice to skip confirmation).
[C 20:31:06.651 NotebookApp] 

```