FROM golang:latest
RUN mkdir /app
ADD . /app/
WORKDIR /app
ENV CGO_ENABLED=0
ENV GOOS=linux
ENV GOPATH=/app:$GOPATH
RUN go get -v github.com/tchaudhry91/rainbow-sha256-go && \
    go build -a -installsuffix cgo github.com/tchaudhry91/rainbow-sha256-go 
ENTRYPOINT [ bash -c "sleep 15;","/app/bin/rainbow-sha256-go"]
