# Python Command Line App Using Click via Alpine Docker Image

## Build new image from DOCKERFILE

- name with a tag

```bash
docker build -t hi .  # Create image using this directory's Dockerfile
```

## Run container

- Remove container when it finishes.
- Run in interactive mode
- Run default or other CMD
- Optionally, provide arguments

```bash
docker run --rm -it hi # run with default CMD from DOCKERFILE
docker run --rm -it hi hello --help # show help
docker run --rm -it hi hello --name David --count 10 # run specified CMD with arguments
```

## Make it useful

Edit the `hello.py` functions and `setup.py` mappings to commands.