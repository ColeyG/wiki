# Setting up an SSL Self-Signed Cert Through NGINX

## Commands

I'd suggest installing the snap version since the current Ubuntu release from the PPA is not working as of 6/17/2020.

- `sudo snap install --beta --classic certbot`
- `sudo certbot --nginx -d colegeerts.com -d www.colegeerts.com -d dev.colegeerts.com`

## Automating Daily Certification Updates

- `crontab -e`
- `0 12 * * * /usr/bin/certbot renew --quiet`
