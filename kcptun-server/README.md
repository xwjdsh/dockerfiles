# kcptun server Dockerfile

* [docker-hub](https://hub.docker.com/r/wendellsun/kcptun-server/)
* [kcptun](https://github.com/xtaci/kcptun)

## Run example
`docker run -d -p 3400:3400/udp --name kcptun-server -e T=10.0.0.1:3389 wendellsun/kcptun-server`

## More option
* `-e T=10.0.0.1:3389` your shadowsocks server address
* `-e MODE=fast3` kcptun server mode,default value is **fast2**

Except these environment variable, other option set with `docker run` command.
eg:
`docker run ..... wendellsun/kcptun-server --key wendell --crypt aes-128`
