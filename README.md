

### Custom Domain Setup
Go to wherever your domain DNS is managed (Namecheap, GoDaddy, Cloudflare, etc.).

### Add A records

Add the following DNS **A records**:

| Type | Name | Value |
|-----|-----|-----|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

These IP addresses are the official **GitHub Pages servers**.

---

### Add WWW support (recommended)

Add the following **CNAME record**:

| Type | Name | Value |
|-----|-----|-----|
| CNAME | www | iranianwomen4internet.github.io |
