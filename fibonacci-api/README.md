### Create account on Docker Hub
Click [here](https://hub.docker.com/) to login

### Docker Labs (Super Lazy Developers)
Click [Lab](https://labs.play-with-docker.com/#) to initialize

### Fibonacci API

Pull the image from Docker Hub using the following command
``` bash
docker pull nishikantpatil/fibonacci-api:0.1
```

Verify the image using the following command 
``` bash
docker images
```
Spin up a container using the following command 
``` bash
docker run -dp host-port:8080 nishikantpatil/fibonacci-api:0.1 
# replace 'host-port' with any unused port on the host machine
```

Verify the container state using the following command
```bash
docker ps
```
Fibonacci API will be available at 
```html
http://localhost:host-port:/fibonacci/get-first-n-fibonnaci-numbers/5
```

Swagger UI will be available at 
```html
http://localhost:host-port:/v3/api-docs
```
Swagger Doc JSON will be available at 
```html
http://localhost:host-port/swagger-ui.html
```
