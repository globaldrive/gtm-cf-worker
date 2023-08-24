# Cloudflare GTM Worker

Used as gtm.domain.com/* Worker route.  
Proxy to prevent blocking GTM by adblockers. 

## Installation

1. Publish this worker with Wrangler.
2. Create Worker Route in your domain config: `gtm.globaldrive.ru/*`
3. Add DNS record. Type: A, Name: gtm, IP: 1.2.3.4 (could be anything), Proxied: true
4. Replace url in GTM script with `https://gtm.globaldrive.ru/?id=`
