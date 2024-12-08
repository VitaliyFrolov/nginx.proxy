### <span style="color: red;">**Warning! This version is under development and is not stable.**</span>
# Nginx Proxy Server
## Proxy server to bypass regional resource blocking

## Technologies:
- Nginx
- Docker

## Commands:
- `build-up` - build and start proxy
- `make down` - down proxy
- `make status` - docker container status

## How to start
1. Copy this project to your VPS server 
2. Add SSL certificates
3. Make sure you have docker installed `Docker -v`
4. Enter the command to build `make build-up`

## Example request
```
curl -k -H "X-Target-Url: https://jsonplaceholder.typicode.com/posts/1" https://<host_name>:443 

```