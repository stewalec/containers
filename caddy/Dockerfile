FROM caddy:builder-alpine AS builder

RUN xcaddy build \
    --with github.com/anxuanzi/caddy-dns-ClouDNS

FROM caddy:alpine

COPY --from=builder /usr/bin/caddy /usr/bin/caddy
