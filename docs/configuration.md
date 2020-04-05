# Configuration

## Docker Basic Configuration

```
NEKO_BIND=0.0.0.0:8080    // Bind
NEKO_CERT=                // (SSL) Cert, needed for clipboard sync
NEKO_KEY=                 // (SSL) Key, needed for clipboard sync
NEKO_PASSWORD=neko        // Password
NEKO_PASSWORD_ADMIN=admin // Admin Password
```

## Environment Variables

* **NEKO_BIND**: socket to bind to.
* **NEKO_CERT**: certificate for SSL.
* **NEKO_KEY**: key for SSL.
* **NEKO_PASSWORD**: the non-administrative user password. Any user authenticating with this will be given non-admin privileges.
* **NEKO_PASSWORD_ADMIN**: the administrative user password. Any user authenticating with this will be given admin privileges.
