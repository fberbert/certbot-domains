# Certbot-Domains

This script lists all domains and subdomains in a Let's Encrypt certificate file.

# Certbot-expand

This script expands your current certificate with new subdomains.

Created by Fábio ([https://mestrefabio.com](https://mestrefabio.com)).

## Instructions

1. Download the script.

2. Make the scripts executable:

```bash
chmod +x certbot-domains
chmod +x certbot-expand
```

3. Copy the scripts to one of your PATH directories, for example:

```bash
sudo cp certbot-domains /usr/local/bin
sudo cp certbot-expand /usr/local/bin
```

## cert-domains

Run the script by passing the domain or folder as a parameter (`/etc/letsencrypt/live/[domain or folder]`):

```bash
sudo certbot-domains mydomain.com
```

The script will list all your domains and subdomains:

```
mydomain.com
mail.mydomain.com
www.mydomain.com
dev.mydomain.com
```

## cert-expand

Run the script by passing the domain or folder as a parameter, and subsequent subdomains.

```bash
sudo certbot-expand mydomain.com www.mydomain.com mail.mydomain.com ...
```

**Note:** You need `sudo` permissions to access the Let's Encrypt local folder.
