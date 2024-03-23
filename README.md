local環境にちょっと構築したいとき用  
homeに永続化用のdirを作っておく


```sh
mkdir -p ~/gitlab/{config,logs,data}
```

```
docker compose up -d
```

gilab/config/gitlab.rbが生成されるので編集する

```ruby
external_url 'http://localhost:8081'
nginx['listen_port'] = 80
```

再度実行
```
docker compose up -d
```