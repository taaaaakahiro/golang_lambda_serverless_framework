# golang_lambda_serverless_framework
## Version
 ```sh
 $ serverless -v
 ```
## Make project
```sh
$ serverless create -u https://github.com/serverless/serverless-golang/ -p [プロジェクト名]
```

## Build
```sh
$ GOARCH=amd64 GOOS=linux go build -o bin/main # for M1
```

## Deploy
```sh
$ cd ./goserverless
$ serverless destroy --region ap-northeast-1 
```

## Destroy
```
$ serverless remove --region ap-northeast-1 
```