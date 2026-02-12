# Step 3: Set Up Professional Email with Zoho

Zoho Mail provides a free, professional email service for your custom domain.

## What You’re Doing
You will configure Zoho Mail as your email provider and verify your domain using Cloudflare DNS.

## Why Zoho
- Forever Free Plan  
- Up to 5 users  
- Excellent deliverability  
- Full support for SPF, DKIM, and DMARC  

## Actions

### 1. Sign Up
Use a personal email address to create your Zoho account.  
Enable MFA immediately.

### 2. Add Your Domain
Zoho will guide you through domain verification.

### 3. Add DNS Records in Cloudflare
You will add:

- **TXT** record for domain verification  
- **MX** records for mail delivery  
- **SPF** record  
- **DKIM** record  
- **DMARC** record (later via EasyDMARC)  

### 4. Create Your First Email Address
Example:
admin@your-cool-lab.qzz.io


Send test emails to confirm delivery.

### 5. Verify SPF, DKIM, and DMARC
Use Zoho’s built-in tools to confirm everything is configured correctly.

## Common Pitfall
Do not let Cloudflare auto-append your domain.  
For example, the DKIM record name should be:
zmail._domainkey

Not:
zmail._domainkey.your-cool-lab.qzz.io
