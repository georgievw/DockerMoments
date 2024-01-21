FROM continuumio/miniconda3

RUN conda create --name my_test

RUN conda env export > environment.yml

RUN pip install geopandas seaborn nltk star