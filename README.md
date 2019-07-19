# darknet_service for YOLOv3

Use [darknet](https://pjreddie.com/darknet/yolo/) object detection from an API:

```shell
docker build -t darknet .
docker run --rm -p 0.0.0.0:3000:3000 --name running-darknet darknet
```

You can request the service with curl like:

```shell
curl -F "photo=@my_photo.jpg" localhost:3000/yolo
curl -F "photo=@my_photo.jpg" localhost:3000/yolo-tiny
curl -F "photo=@my_photo.jpg" localhost:3000/yolo-voc
```

Read more about darknet <https://pjreddie.com/darknet/yolo/>
