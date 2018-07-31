FROM golang:latest

RUN go get -d -v github.com/otrv4/otrng-prekey-server/server/raw
RUN go install -v github.com/otrv4/otrng-prekey-server/server/raw
RUN go env GOPATH

ENTRYPOINT ["/go/bin/raw"]
CMD ["-h"]
