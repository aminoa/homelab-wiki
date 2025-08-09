# Software

All my servers run Fedora 42 (I like its reliable package manager and generally up-to-date packages). The cluster uses k3s on top. The internal websites are accessed using Tailscale. The public facing websites use Cloudflare Tunnels (it makes the software stack simpler since I don't need to set up a reverse proxy or certificates). 

TODO: publish kubernetes configs in a separate repo
