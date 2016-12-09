# SS Dockerfile

* [docker-hub](https://hub.docker.com/r/wendellsun/shadowsocks-go/)
* [shadowsocks-go](https://github.com/shadowsocks/shadowsocks-go)

## Run example:
`docker run -d -p 3389:3389 --name ss -e K=password wendellsun/shadowsocks-go`

## More option:
* `-e K=password` your shadowsocks server password 
* `-e M=aes-128-cfb` encryption method,default value is **aes-256-cfb**
* `-e T=30` timeout,in seconds,default value is **60**

Except these environment variable, other option set with `docker run` command.
eg:
`docker run ..... wendellsun/shadowsocks-go -d -c config.json`
