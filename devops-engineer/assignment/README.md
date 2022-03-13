### Docker build image and run
After cloning the repository
Run

```sh
docker build -t httpserver .
```

```sh
docker run -itd -p 8080:8080 httpserver
```

Access with localhost with port , In my case i access with public ip associated with my instance.

Also image pushed to [dockerhub](https://hub.docker.com/r/sandeepdocker45/httpserver)

### Issues
Unable to install kubernetes because of hardware limitations

For Task no-3
It is required to have data .wav files to write & test according to script.  
