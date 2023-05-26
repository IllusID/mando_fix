## Prerequisites
- [docker](https://docs.docker.com/engine/install/)
- [node](https://nodejs.org/en/download/) 16.15.1 or higher
- [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) 8.11.0 or higher

## Deploy on Local Machine

** Activate environment
```
source mando-env/bin/activate
```

### Backend
- Pull docker image from docker hub:
```
docker pull nguyenminh1807/sco:latest
```

- Run container:
```
docker run -it -d --rm  --name sco_app -p 5555:5555 nguyenminh1807/sco:latest
```

### Frontend
- Navigate to frontend directory:
```
cd sco_frontend
```

- Launch app from local:
```
npm start
```
