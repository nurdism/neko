# Setup Caddy and Neko
This guide assumes you already have Caddy and Neko installed, and that you have confirmed Neko is working over the standard port.

After completing this guide, you will have setup a reverse proxy from Caddy to Neko, and you will have enabled TLS support.

It took me a bit of Googling around, but the config you need to add is pretty straight forward.

```
https://neko.example.com {
  reverse_proxy localhost:8080 {
    header_up Host {host}
    header_up X-Real-IP {remote_host}
    header_up X-Forwarded-For {remote_host}
    header_up X-Forwarded-Proto {scheme}
  }
}
```

Go ahead and add that snippet to your Caddyfile (usually at /etc/caddy/Caddyfile), and then (re)start Caddy to have the changes go into effect.

Remember to set your DNS records properly so Caddy can talk with Let's Encrypt, and have fun!
