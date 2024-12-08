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
2. Make sure you have docker installed `Docker -v`
3. Enter the command to build `make build-up`

## Example request
```
curl -X POST http://your-vps-ip:3000 \
-H "Content-Type: application/json" \
-H "X-Target-Url: https://api.openai.com/v1/chat/completions" \
-d '{"model": "gpt-3.5-turbo", "messages": [{"role": "user", "content": "Hello!"}]}'

```