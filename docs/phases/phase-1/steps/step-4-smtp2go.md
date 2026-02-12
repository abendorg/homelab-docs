# Step 4: Configure an Email Relay with SMTP2GO

Your homelab applications (Nextcloud, Portainer, etc.) cannot send email directly from your home IP.  
SMTP2GO solves this by relaying mail through trusted servers.

## What You’re Doing
You will verify your domain with SMTP2GO and configure it as your outbound relay.

## Why SMTP2GO
- Free plan with 1,000 emails/month  
- Excellent deliverability  
- Required for application notifications  
- Works seamlessly with Zoho  

## Actions

### 1. Create an Account
Sign up and enable MFA.

### 2. Verify Your Domain
SMTP2GO will provide **three CNAME records**.  
Add them in Cloudflare.

### 3. Create SMTP Credentials
Generate a username/password or API key.  
Store these in your password manager.

### 4. Use These Credentials Later
In Phase 4, nearly every container will use SMTP2GO for:

- Password resets  
- Alerts  
- Notifications  
- System messages  

## Tip
Use port **587** with **STARTTLS** for most applications.