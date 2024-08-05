# alpine-php-7.2
## 构建命令
```
docker build -t registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-latest .
```

## 运行命令
```
docker run -d -p 8080:80 --name test registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-latest
```

## 进入容器
```
docker exec -it test sh
```

## 推送仓库
```
docker push registry.cn-hongkong.aliyuncs.com/stevennight-test/registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-latest
```

# alpine-php-7.2-dev

## 构建命令
```
docker build -f Dockerfile-dev -t registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-dev-latest .
```

## 运行命令
```
docker run -d -p 8080:80 --name test registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-dev-latest
```

## 进入容器
```
docker exec -it test sh
```

## 推送仓库
```
docker push registry.cn-hongkong.aliyuncs.com/stevennight-test/alpine-php:7.2-dev-latest
```

## 环境变量
- XDEBUG_CLIENT_HOST：xdebug 客户端地址（php.ini xdebug.client_host）
- PHP_IDE_CONFIG：xdebug ide配置环境变量（官方Docker）
