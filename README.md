# Colton's Docker Stuff and Stuff

- Jupyter

    1. Clone Repo `git clone https://github.com/Schneeple/home.git`
    2. Go into the directory `cd home/docker/jupyter/`
    3. Build the docker image `docker build -t coltonjupyter -f Dockerfile .`
    4. Naviagte to where you the notebooks to save to in terminal and run: `docker run -d -p 10000:8888 -v "$PWD":/home/jovyan/work coltonjupyter`
    5. Use `docker ps -a` to get the docker tag and insert it in place of `
    <tag>` in the follow command `docker logs <tag>` to get the url and token.


