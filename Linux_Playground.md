# Setup a linux playground to practice bash commands

This section will cover two options to set up a Linux environment for practicing:

You have two options:

1. [Set up the Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install)
2. Use a Docker container (See instruction below on how to create, build and run a `Dockerfile`)

## Create the `Dockerfile`
Save the following content as a file named `Dockerfile`
```yml
FROM ubuntu:latest
CMD tail -f /dev/null
```
This Dockerfile is intentionally simple to demonstrate the core concepts. You can customize it by 
- Choosing a different base image (e.g., `alpine`, `debian`).
- Setting a different default command (e.g., `CMD ["python", "-m", "http.server"]`).
- Adding more instructions to install software or configure the container environment.

>`tail -f /dev/null` acts as a placeholder process that keeps the container running without consuming.resources.

## Build the docker image:
    docker build -t my-linux-container .

## Run the docker container in interactive mode:
    docker run -it my-linux-container bash

## Check it worked with `uname -a`

The `uname -a` command prints system information about the operating system running in the container.

Specifically:
- `uname` stands for "Unix Name".
- `-a` is the argument that tells uname to print all available system information.
- Without any arguments, uname only prints the operating system name.