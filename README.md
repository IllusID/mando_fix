## Prerequisites
- [docker](https://docs.docker.com/engine/install/)
- [node](https://nodejs.org/en/download/) 16.15.1 or higher
- [npm](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) 8.11.0 or higher

## Deploy on Local Machine

### Activate environment
```
source mando-env/bin/activate
```
(You might be wondering at this point why I am not removing the env folder because I don't want to resolve those issues or utilize the deprecated library or wait for the libraries installation. I simply want to clone and run in my computer. That's all!)

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
