# Step 6: Secure Your Home Network with OpenDNS

OpenDNS provides network-wide DNS filtering and security.

## What You’re Doing
You will configure your home router to use OpenDNS instead of your ISP’s DNS.

## Why OpenDNS
- Blocks malware and phishing  
- Adds a security layer before Pi-hole  
- Protects every device on your network  

## Actions

### 1. Create an Account
Sign up for OpenDNS Home Free.

### 2. Update Your Router’s DNS Settings
Set:
Primary DNS:   208.67.222.222 Secondary DNS: 208.67.220.220


### 3. Link Your Network
Add your home IP address in the OpenDNS dashboard.

### 4. Install the Dynamic IP Updater
Your home IP changes.  
The updater keeps OpenDNS linked to your network.

### 5. Configure Filtering
Enable:

- Malware/Botnets  
- Phishing  
- Suspicious Responses  

Optional categories depend on your household.

## Pi-hole Later
OpenDNS is your outer wall.  
Pi-hole becomes your inner wall in Phase 4.