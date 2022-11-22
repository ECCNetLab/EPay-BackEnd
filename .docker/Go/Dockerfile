# ベースとなるDockerイメージ指定
FROM golang:latest

# コンテナログイン時のディレクトリ指定
WORKDIR /go/src/work

RUN curl -sSfL https://raw.githubusercontent.com/cosmtrek/air/master/install.sh | sh -s -- -b $(go env GOPATH)/bin

EXPOSE 9000
