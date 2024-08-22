# Fivem-Proxy-Install.sh
This is a handy script made by MathiAs2Pique to install Nginx as a proxy for your FiveM/RedM server. I take no credit for this; it was created by MathiAs2Pique. I just made a couple of modifications to support Ubuntu. This script is incredible and makes setting up a proxy so easy. 

As you know, having a proxy for your FiveM server is very important and a great way to avoid getting DDoS attacks and users discovering your public IP. This can also be set up with Cloudflare Tunnel, but only do this if you know what you're doing. This script is perfect for setting up the reverse proxy. If you have any questions or need help, please create an issue.

## Requirements
- Debian linux distribution (Tested on debian 10/11)
- Root access
- A domain name
- A FiveM/RedM server

## Installation

**Side Note:** Make sure you have your domain ready and pointing to the server IP if you're going to use SSL. If you're unsure what this means, it involves creating an A record for the specific hostname you will be using. For example, if your hostname is `play1.mydomain.com`, you would create an A record that points to the server IP. This is necessary so that CERTBOT can generate your SSL certificate. You need to do this before you start the install script.

1. Download the script (git clone https://github.com/apeoplerson/Fivem-Proxy-Install.sh.git fivemproxy)
2. cd into fivemproxy folder (cd fivemproxy)
3. Make it executable: `chmod +x fivem-nginx-proxy-install.sh`
4. Run it: `./fivem-nginx-proxy-install.sh`

## Usage
1. Follow the instructions
2. Enjoy your new proxy!

## Credits
- [Nginx](https://nginx.org/)
- [Certbot](https://certbot.eff.org/)
- [Let's Encrypt](https://letsencrypt.org/)
- [FiveM](https://fivem.net/)
- [RedM](https://redm.gg/)
- [MathiAs2Pigue](https://github.com/MathiAs2Pique)

## Additional notes by MathiAs2Pique
- I personnaly recommend to use CloudFlare: DNS, Proxy and Edge Cache are really useful. 
- Please do not use the built-in nginx cache, as it's a mess if you want to udpate your scripts, and it would cost you a lot more than CloudFlare.
- If you have your own SSL certificate, then just check web.conf to edit what needs to be edited.
- If you want to use a custom port, then just check web.conf to edit what needs to be edited.
- A **single** proxy is **not useful at all** as a DDoS protection, but it can be useful to hide your IP address.
