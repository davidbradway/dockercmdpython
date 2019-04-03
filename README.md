# Python Command Line App Using Click via Alpine Docker Image

## Build new image from DOCKERFILE

```bash
docker build -t hi .  # Create image using this directory's Dockerfile
```

## Run command "hello" with arguments in container

```bash
docker run --rm -it hi # run with default CMD from DOCKERFILE
docker run --rm -it hi hello --help # show help
docker run --rm -it hi hello --name David --count 10 # run specified CMD with arguments
```

## Make it do something useful

Edit the `hello.py` functions and `setup.py` mapping to commands.