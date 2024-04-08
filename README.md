local環境にちょっと構築したいとき用  
homeに永続化用のdirを作っておく


```sh
mkdir -p ~/gitlab/{config,logs,data}
```

```
docker compose up -d
```

webui
```
root
passwordはrails cしてからかえたほうがいい
```


rails cの代替
```
docker exec -it gitlab-docker-web-1 bash
gitlab-rails c
```