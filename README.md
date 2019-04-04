# Python Command Line App Using Click via Alpine Docker Image


- Click allows one to make nice Python CMD apps, but you would need to install it in a virtualenv and activate it to use
- So I created a using a Python 3 Alpine Docker Image https://github.com/davidbradway/dockercmdpython
- So now you just create a Docker image and run the command line apps in a container

## Build new image from DOCKERFILE

- give it a tag "hi"

```bash
docker build -t hi .  # Create image using this directory's Dockerfile
```

## Run container

- Remove container when it finishes
- Run interactive, tty mode
- Run default or other command
- Optionally, provide arguments

```bash
docker run --rm -it hi # run with default CMD from DOCKERFILE
docker run --rm -it hi hello --help # show help
docker run --rm -it hi hello --name David --count 10 # run specified CMD with arguments
```

## Make it useful

Edit the `hello.py` functions and `setup.py` mappings to commands.