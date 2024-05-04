# Certbot-Domains

This script lists all domains and subdomains in a Let's Encrypt certificate file.

Created by Fábio ([https://mestrefabio.com](https://mestrefabio.com)).

## Instructions

1. Download the script.

2. Make the script executable:

```bash
chmod +x certbot-domains
```

3. Copy the script to one of your PATH directories, for example:

```bash
sudo cp certbot-domains /usr/local/bin
```

4. Run the script by passing the domain or folder as a parameter (`/etc/letsencrypt/live/[domain or folder]`):

```bash
sudo certbot-domains mydomain.com
```

5. The script will list all your domains and subdomains:

```
mydomain.com
mail.mydomain.com
www.mydomain.com
dev.mydomain.com
```

**Note:** You need `sudo` permissions to access the Let's Encrypt local folder.
