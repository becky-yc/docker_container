# container-from-scratch-python
This is building a container from scratch

## Build the Container Yourself and Push to Docker Hub

### Build image
*(If you want to develop yourself)* 
docker build --tag=test_hello_hello .

### List docker images
docker image ls

### Run my newly built container

docker run -it test_hello_hello python app.py --name "Big John"

### Push to Docker Hub

*Note:  You will need to change for your Docker Hub Repo*
docker push mishamiho/test_hello_hello:tagname

## Run it yourself

```bash
docker pull mishamiho/test_hello_hello:latest
docker run -it mishamiho/test_hello_hello bash 

#then run python app.py --help
```

## Pass in a command

```bash
docker run -it mishamiho/test_hello_hello python app.py --name "Big John"
#the output
Hello Big John!
```

