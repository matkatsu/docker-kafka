# 概要
kafka検証用docker環境です。
zookeeper,kafka共にシングルノードです。

## 起動
```
$ docker-compose up -d
```

### Kafka UI Tool

[http://localhost:8000](http://localhost:8000)

## 停止
```
$ docker-compose down
```

# Go クライアントサンプル
## 事前準備(Mac)
### 1. librdkafkaのインストール
```
$ brew install librdkafka
```
`pkg-config`も無ければinstallしてください。

### 2. hosts設定
`/etc/hosts`に以下を追加してください。
```
127.0.0.1 kafka
```

### 3. glide install
```
$ glide install
```

## Producer
```
$ go run main.go
```

## Consumer
準備中...
