# Docker slow dns response

Each dns request will  have a very slow response, 5seconds, and always with the
same IP 192.168.0.2

To run:

```
$ docker build -t my-golang-app .
$ docker run -it --rm -p 53:53 --name my-running-app my-golang-app
```
