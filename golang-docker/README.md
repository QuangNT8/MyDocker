
This is an example about how to install golang to docker image.

```Remove all docker images
$ docker image prune
```
```
### Build the app’s container image
``` Build with tag name is golang
$ docker build -t golang .
```
```
``` login 
$ docker login -u quang102
```
``` docker tag
$ docker tag golang quang102/myprojects:golang
```
### Push the image
``` docker push
$ docker push quang102/myprojects:golang
``` 
```
### EOF


