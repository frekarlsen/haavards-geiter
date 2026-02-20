# 🐐 Håvards Geiter

Nettside for Håvards gard — geiter, epler, cider og traktor.

## Deploy på Unraid

```bash
cd /mnt/user/appdata
git clone https://github.com/frekarlsen/havards-geiter.git
cd havardsgeiter
docker compose up -d --build
```

## Oppdatering

```bash
cd /mnt/user/appdata/havardsgeiter
git pull
docker compose up -d --build
```

## Cloudflare Tunnel

Legg til public hostname i Cloudflare Zero Trust:
- **Subdomain:** geiter (eller kva du vil)
- **Domain:** frekar.no
- **Service:** http://haavards-geiter:80
