FROM jupyter/datascience-notebook

USER root

RUN apt-get update && \
    apt-get install -yq \
        fonts-mplus \
        && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Switch back to jovyan to avoid accidental container runs as root
USER $NB_UID

RUN pip install wordcloud pandas
