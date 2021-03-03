
# How To Run
# docker build -t jupyter -f Dockerfile .
# docker run -d -p 10000:8888 -v "$PWD":/home/jovyan/work jupyter



FROM jupyter/datascience-notebook

WORKDIR /opt/conda/lib/python3.8/site-packages
RUN /bin/bash -c "git clone https://github.com/DidierRLopes/GamestonkTerminal.git"

ENV JUPYTER_ENABLE_LAB=yes

EXPOSE 8888
WORKDIR "/home/jovyan/work"

# docker run -d -p 10000:8888 -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan/work jupyter/datascience-notebook