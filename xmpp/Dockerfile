FROM golang:latest

RUN go get -d -v github.com/otrv4/prekey-server-xmpp
RUN go install -v github.com/otrv4/prekey-server-xmpp
RUN go env GOPATH

ENTRYPOINT ["/go/bin/prekey-server-xmpp"]
CMD ["-h"]
