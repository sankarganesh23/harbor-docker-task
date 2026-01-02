# harbor-docker-task
Xeon AI DevOps Task: Docker Harbor Wordcount Challenge  Built Docker image harbor-task-wordcount:latest from Python 3.13-slim base. Fixed WSL chmod issues, Dockerfile COPY/RUN order, BuildKit output. Image tested successfully with docker run.
# Xeon AI Docker Harbor Task

## Status
✅ Dockerfile complete  
✅ solve.sh executable  
✅ Image built: `harbor-task-wordcount:latest`

## Commands
```bash
cd /mnt/e/harbor_tasks
sudo docker build -f environment/Dockerfile -t harbor-task-wordcount .
sudo docker run --rm harbor-task-wordcount

**DockerFile**
FROM python:3.13-slim
WORKDIR /app
COPY solution/solve.sh /app/solve.sh
RUN chmod +x /app/solve.sh

**Verification**
$ sudo docker images | grep harbor-task-wordcount
harbor-task-wordcount  latest  ✓

$ sudo docker run --rm harbor-task-wordcount
✓ Runs successfully

Submitted to Xeon AI
shivlaktraya@xeon.ai
