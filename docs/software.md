# Software

This will discuss non-service related software. All my laptops run Fedora 43 (I like its reliable package manager and generally up-to-date packages) with k3s on top. Traefik reverse proxies traffic from public subdomains into specific Kubernetes services. 

![Fedora](./assets/Fedora.jpgj)

## Access 

I use Cloudflare domains for all my public endpoints and Cloudflare's proxy to help protect my laptops from DDOS attacks. I access my private websites via Tailscale directly with no subdomains.

## Security

I use Sealed Secrets to track various secrets in code. I also monitor my cluster using Headlamp (the desktop app).

## Storage

Longhorn is used for distributed storage for CTFd and ROMM. I use one main storage class: `longhorn-main`. It creates two replicas and attempts to schedule pods closer to its data. 

## Dynamic DNS 

I don't have a static IP so I used [cloudflare-ddns](https://github.com/timothymiller/cloudflare-ddns) to periodically update my DNS A subdomain records to point at my current public IPv4 IP. 
