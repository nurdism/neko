# Configuration

## Docker Basic Configuration

```
NEKO_ADMIN=admin        // Admin Password
NEKO_BIND=0.0.0.0:8080  // Bind
NEKO_CERT=              // (SSL) Cert, needed for clipboard sync
NEKO_KEY=               // (SSL) Key, needed for clipboard sync
NEKO_PASSWORD=neko      // Password
```

## Environment Variables

* **NEKO_ADMIN**:  the administrative user password. Any user authenticating with this will be given admin privileges.
* **NEKO_BIND**:  socket to bind to.
* **NEKO_CERT**:  certificate for SSL.
* **NEKO_KEY**:  key for SSL.
* **NEKO_PASSWORD**:  the non-administrative user password. Any user authenticating with this will be given non-admin privileges.
