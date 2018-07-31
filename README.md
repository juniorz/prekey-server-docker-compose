# Running a prekey server on Docker

This is to give some inspiration on what needs to be put together.

```
git clone this
cp .env-sample .env
edit .env
docker-compose up
```

On my setup, I have a XMPP server that listen for connections on
`/run/prosody-components.so`. I have to use a socat container to expose this
inside the docker network bc the XMPP prekey server does not handle unix
sockets.

If you run everything on docker, you shoudl not have that problem.
