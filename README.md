# redis

## 父镜像地址
```shell script
https://github.com/docker-library/redis/blob/1d6d5acf99aedd42aa0195ad5f22b8ffa6841f96/4.0/Dockerfile
```
## 镜像信息
```shell script

https://cr.console.aliyun.com/repository/cn-beijing/meowbite/redis/build

registry.cn-beijing.aliyuncs.com/meowbite/redis:4.0.1

```

## 使用方法
```shell script
docker pull registry.cn-beijing.aliyuncs.com/meowbite/redis:4.0.1

docker run --name some-redis -p 6379:6379 -v /my/own/datadir:/data -d registry.cn-beijing.aliyuncs.com/meowbite/redis:4.0.1
```

## 参考dockerfile
```bash
https://c.163yun.com/hub#/library/repository/info?repoId=2973
```

## 验证

```shell script
docker exec  -it b9d2b1cc736b bash
root@b9d2b1cc736b:/data# redis-cli
127.0.0.1:6379> set abc 123
OK
127.0.0.1:6379> get abc
"123"
127.0.0.1:6379>
```