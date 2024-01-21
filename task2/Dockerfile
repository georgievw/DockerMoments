FROM continuumio/miniconda3

RUN conda create --name my_test

RUN git clone --depth 1 https://github.com/geopandas/geopandas.git \
    && cd geopandas \
     &&pip install .

RUN git clone --depth 1 https://github.com/mwaskom/seaborn.git \
    && cd seaborn \
    && pip install .

RUN git clone --depth 1 https://github.com/nltk/nltk.git \
    && cd nltk \
    && pip install .

RUN git clone --depth 1 https://github.com/dbrgn/star.git \
    && cd star \
    && pip install star


