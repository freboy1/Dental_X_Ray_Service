# Dental_X_Ray_Service 

Simple API for object detection using YOLO + FastAPI, containerized with Docker.

---

## Requirements

- Docker version 27.3.1, build ce12230
- Docker Compose version v2.30.3-desktop.1

---

## Run Project

### Build and start containers

```bash
docker build -t yolo-api .
docker run -p 8000:8000 yolo-api
````

---

## Access Application

After starting, the API will be available at:

```
http://localhost:8000/docs
```

---

## Stop Project

### Stop running container

```bash
docker ps
docker stop <container_id>
```

---

## Notes

* Upload image via `/predict` endpoint
* YOLO model runs inference and returns detections with bounding boxes
* Default port: `8000`

