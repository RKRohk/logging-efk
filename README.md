# logging-efk

### A set of tools that will help you set up your own logging infrastructure

## Prerequisites

- Docker
- Docker-compose
- A [Cloudflare] account with cloudflared enabled for remote access

[Cloudflare]: https://cloudflare.com

## How to use

1. Clone the repo
2. Run `docker-compose up -d`
3. Set up cloudflared zero trust and point a subdomain to http://kibana:5601
4. Done!