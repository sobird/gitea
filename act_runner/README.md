# act_runner

```sh
# 启动 act_runner

docker run -d 
  --restart always 
  --name act_runner 
  -e CONFIG_FILE=/data/config.yaml 
  -e GITEA_INSTANCE_URL=http://192.168.50.100:3000/ 
  -e GITEA_RUNNER_REGISTRATION_TOKEN=tOCwFvUOIFYzQCnc7MVt3z0OwEewLAhTUyZ4TUTv 
  -e GITEA_RUNNER_NAME=act_runner_windows 
  -v ./data:/data 
  -v /var/run/docker.sock:/var/run/docker.sock 
  gitea/act_runner:latest
```