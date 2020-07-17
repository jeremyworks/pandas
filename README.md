# jeremyworks/pandas
[Jupyter](https://jupyter.org/) notebooks, samples, and resources for processing data in [pandas](https://pandas.pydata.org/docs/)

Code samples can easily be run if you have [Docker](https://www.docker.com/) installed.


# Parsing JSON
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