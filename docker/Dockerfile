ARG SCIPY_NOTEBOOK_VERSION=ea01ec4d9f57
FROM jupyter/scipy-notebook:$SCIPY_NOTEBOOK_VERSION

LABEL maintainer="jeremyworks.com <code@jeremyworks.com>"

USER $NB_UID

RUN conda install --quiet --yes \
    'genson=1.1.0' \
    'xmltodict=0.12.0'