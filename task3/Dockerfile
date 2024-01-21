FROM python
USER root
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    && \
    rm -rf /var/lib/apt/lists/*

ENV VIRTUAL_ENV=/opt/my_test

RUN python3 -m venv $VIRTUAL_ENV
ENV PATH="$VIRTUAL_ENV/bin:$PATH"

RUN pip install --upgrade pip && \
pip install jupyter geopandas seaborn nltk STAR

EXPOSE 8888

ENTRYPOINT ["jupyter","notebook","--ip=0.0.0.0","--allow-root"]


