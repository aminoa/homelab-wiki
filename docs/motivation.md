# Motivation

## History

I've had various forms of a homelab for the past three years. In 2023, I ran a ThinkPad X1 individually and run multiple private services (Jellyfin, Portainer, miniflux, etc.) accessed via Tailscale. I later expanded to using Cloudflare Tunnels to serve CTFd publically. 

I didn't come back to my homelab until late 2024 when my G14 screen stopped working and I had to get a new laptop. Since I now had three laptops (my dad's old ThinkPad, my previous ThinkPad, and the G14), I decided to make a basic k3s cluster. I hyperfocused on getting Ceph working (big mistake) and ended up losing motivation. I created a Digital Ocean VPS that I hosted CTFd on to keep that sight running while I tabled my homelab again.

In mid-2025, I moved to a new apartment in NY and, over a couple months, wired my computers back up. Now in 2026, a couple weeks ago, I wanted to finally strike this project off the bucketlist. I decided to focus far more on providing public services since I found it more useful and fun. With time and tokens, I moved a lot of websites onto my cluster (including emptypad, originally GH pages, and CTFd, origianlly Digital Ocean) and set up deployments for a lot of older personal projects.

## Rationale

1) Pay respect to the computers that have served me for years and get a few more cycles out of them before they pass

2) Showcase interesting projects I've worked on in an accessible manner (ex. DAC web port)

3) Provide services that would be more cumbersome to run on my laptop/phone (ex. ROMM)