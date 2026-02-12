# Troubleshooting — Phase 1

Most issues in this phase fall into a few predictable categories.  
Patience is your most important tool.

---

## DNS Records Not Found

### Cause: Propagation Delay
DNS changes take time.

### Fix
- Wait 5–15 minutes  
- Check with dnschecker.org  
- Verify record names are correct  

---

## Incorrect Record Names

Cloudflare auto-appends your domain.  
Ensure you are not duplicating it.

Example:
Correct: zmail._domainkey Wrong:   zmail._domainkey.your-cool-lab.qzz.io


---

## Cloudflare Proxy Enabled

Email-related records must be **DNS-only** (grey cloud).

---

## Email Going to Spam

### Cause
SPF or DKIM misconfigured.

### Fix
- Re-check Zoho’s SPF builder  
- Re-copy DKIM record  
- Verify in Zoho’s dashboard  

---

## OpenDNS Not Blocking

### Cause 1: DNS Cache
Flush DNS or restart your device.

### Cause 2: IP Address Changed
Ensure the Dynamic IP Updater is running.

---

## Locked Out Due to MFA

Use your backup codes.  
If you didn’t save them, you must go through account recovery.

---

## SMTP2GO Relay Issues

- Use port 587 with STARTTLS  
- Verify domain in SMTP2GO  
- Check logs for rejected messages  

---

## DMARC Reports Not Appearing

- Ensure `_dmarc` record is correct  
- Wait 24–48 hours  
- Send test emails  