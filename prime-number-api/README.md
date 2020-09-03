### Create account on Docker Hub
Click [here](https://hub.docker.com/) to login

### Docker Labs (Super Lazy Developers)
Click [Lab](https://labs.play-with-docker.com/#) to initialize

### Prime Number API

Pull the image from Docker Hub using the following command
``` bash
docker pull nishikantpatil/prime-number-api:0.1
```

Verify the image using the following command 
``` bash
docker images
```
Spin up a container using the following command 
``` bash
docker run -dp 8081:8080 nishikantpatil/prime-number-api:0.1 
# replace 'host-port' with any unused port on the host machine
```

Verify the container state using the following command
```bash
docker ps
```
Fibonacci API will be available at 
```html
http://localhost:host-port:/primes/is-prime/5
```

Swagger UI will be available at 
```html
http://localhost:host-port:/v3/api-docs
```
Swagger Doc JSON will be available at 
```html
http://localhost:host-port/swagger-ui.html
```
