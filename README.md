# Angular Example App

[Demo Website](https://angular.realworld.io)


## Local setup

```bash
# Install the dependencies:
npm install

# Start the server
ng serve
```

Navigate to [http://localhost:4200/](http://localhost:4200/) in your browser


## Docker setup

```bash
# Build the container
docker build -t angularsample:latest .

# Run the container
# --rm  Removes the container when it exits. Useful when experimenting to prevent dozens of containers.
# -p    Maps the ports
# -it   Interactive session to keep the container running
docker run -p 4200:8080 --rm -it angularsample:latest

# Interactive shell session into the container. Useful when you want to debug the container
docker run -p 4200:8080 --rm -it --entrypoint /bin/sh angularsample:latest
```
