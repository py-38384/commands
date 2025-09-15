
Install cloudflared

    sudo apt install cloudflared

Check Version

    cloudflared --version

Start login (note: domain require meaning money require)

    cloudflared tunnel login

Create a tunnel (note: after login)

    cloudflared tunnel create my-tunnel

Start a quick tunnel

    cloudflared tunnel --url http://localhost:3000