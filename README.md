# Jupyter Docker Stacks

## Quick Start

It then starts a container running a Jupyter Notebook server and exposes the
server on host port 8888. The server logs appear in the terminal.
Visiting `http://<hostname>:8888/?token=<token>` in a browser loads the Jupyter
Notebook dashboard page, where `hostname` is the name of the computer running
docker and `token` is the secret token printed in the console. Docker destroys
the container after notebook server exit, but any files written to `~/work` in
the container remain intact on the host.

    docker-compose up
