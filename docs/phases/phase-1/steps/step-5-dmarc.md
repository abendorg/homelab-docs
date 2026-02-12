# Step 5: Monitor Email Security with EasyDMARC

DMARC protects your domain from spoofing and gives you visibility into who is sending mail on your behalf.

## What You’re Doing
You will configure DMARC monitoring using EasyDMARC’s free plan.

## Why EasyDMARC
- Clear dashboards  
- Aggregated reports  
- Forensic reporting  
- Helps validate SPF and DKIM  

## Actions

### 1. Create an Account
Enable MFA immediately.

### 2. Add Your Domain
EasyDMARC will analyze your DNS and generate a DMARC record.

### 3. Add the DMARC Record in Cloudflare
Example:
Type: TXT Name: _dmarc Value: v=DMARC1; p=none; rua=mailto:xxxx@ag.easydmarc.com; ruf=mailto:xxxx@fo.easydmarc.com


### 4. Wait for Reports
DMARC reports take **24–48 hours** to appear.

## Understanding the Policy
- `p=none` — monitoring mode  
- `rua` — aggregate reports  
- `ruf` — forensic reports  

You will tighten this policy in later phases.