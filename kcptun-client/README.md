# kcptun client Dockerfile

[docker-hub](https://hub.docker.com/r/wendellsun/kcptun-client/)
[kcptun](https://github.com/xtaci/kcptun)

## Run example
`docker run -d -p 3500:3500 --name kcptun-client -e R=10.0.0.1:3400 wendellsun/kcptun-client`

## More option
* `-e R=10.0.0.1:3400` your kcptun server address
* `-e MODE=fast3` kcptun server mode,default value is **fast2**

Except these environment variable, other option set with `docker run` command.
eg:
`docker run ..... wendellsun/kcptun-client --key wendell --crypt aes-128`
