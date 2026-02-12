# Step 2: Take Control of DNS with Cloudflare

Cloudflare will manage your DNS, security, and traffic routing.  
It becomes the central control panel for your domain.

## What You’re Doing
You will add your new domain to Cloudflare and delegate DNS authority to them.

## Why Cloudflare
- Free, fast, globally distributed DNS  
- Excellent security features  
- Easy DNS record management  
- Required for later phases (reverse proxies, tunnels, SSL, etc.)  

## Actions

### 1. Create a Cloudflare Account
Sign up at Cloudflare and enable MFA immediately.

### 2. Add Your Domain
1. Click **Add a Site**  
2. Enter your `.qzz.io` domain  
3. Cloudflare will scan for existing DNS records (there won’t be many)

### 3. Update Nameservers
Cloudflare will provide two nameservers, such as:
sue.ns.cloudflare.com tom.ns.cloudflare.com

Go back to the FreeDomain registrar and replace the existing nameservers with Cloudflare’s.

### 4. Wait for Propagation
DNS changes take time.  
Cloudflare will email you when the domain is active.

### 5. Verify DNS Propagation
Use:

- dnschecker.org  
- whatsmydns.net  

Check TXT, MX, and CNAME records as you add them later.

## Important
Cloudflare’s **orange cloud proxy must be disabled** (set to DNS-only) for all email-related records.