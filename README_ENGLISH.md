# edge-tunnel

[简体中文](https://github.com/ImLTHQ/edge-tunnel/blob/main/README.md) | English

This is a script based on the Cloudflare platform.

I am a beginner, so please feel free to point out any problems with the code.

Give it a star before you leave!
[![Stargazers over time](https://starchart.cc/ImLTHQ/edge-tunnel.svg?variant=adaptive)](https://starchart.cc/ImLTHQ/edge-tunnel)

# Usage

Please register for `GitHub` and `Cloudflare` accounts first (CF for short below).

- Fork this project on GitHub first.
- In the CF console, select `Workers`.
- Click `Create` and choose `Workers` or `Pages`.
- For Pages, click `Connect to Git`.
- Select the `edge-tunnel` project and modify the `Name` at the top.
- Add `Variables` according to the `Variable Description` below.
- Click `Save and Deploy`.
- It will not be available immediately after deployment; it takes about 10 minutes to be accessible.
- It will not be available immediately after deployment; you need to wait about 10 minutes.
- Import the subscription address `https://your_domain/subscription_path` into your Clash/V2Ray client.

<details>
<summary><code><strong>「 Recommended Actions After Deployment 」</strong></code></summary>

Set up GitHub Action:
- Go to your forked repository.
- In the `Actions` tab, click the `green button`.
- Choose `Sync upstream`.
- Click `Enable workflow`.
- This is to keep your repository synchronized with the author's latest updates.
</details>

<details>
<summary><code><strong>「 Binding a Custom Domain (Optional) 」</strong></code></summary>

Connect your domain to CF:
- Go to the `Account Home`, select `Domains`, enter your domain, and click `Continue`.
- Choose a plan according to your needs (the free one is sufficient), click `Continue`, click `Continue to activation`, and click `Confirm`.
- Follow CF's instructions to return to your domain registrar and replace your current DNS servers with CF DNS servers.

Bind a custom domain to Pages:
- Click the `Custom domain` tab in the Pages console, click `Set up a custom domain`.
- Enter your domain.
- Click `Continue`, click `Activate domain`.
</details>

# Variable Description

| Variable Name | Example | Remarks |
|-|-|-|
| SUB_PATH | `sub` | Subscription path (supports Chinese) |
| SUB_UUID | `550e8400-e29b-41d4-a716-446655440000` | UUID for verification |
| TXT_URL | `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/HKG.txt` | URL of the TXT file containing preferred IPs. Supports multiple addresses, separated by newlines. Format: address:port#node_name.  If the port is not specified, the default is 443. If the node name is not specified, the default node name is used. |
| SUB_NAME | `Node` | Default node name |
| PROXY_IP | `ts.hpc.tw:443` | Proxy IP |
| SOCKS5_GLOBAL | `true`,`false` | Enable SOCKS5 global proxy |
| SOCKS5 | `username:password@address:port` | SOCKS5 |
| FAKE_WEB | `baidu.com` | Fake website for the root path |

<details>
<summary><code><strong>「 More ProxyIPs 」</strong></code></summary>

- `ts.hpc.tw`
- `ProxyIP.US.CMLiussss.net`
- `ProxyIP.SG.CMLiussss.net`
- `ProxyIP.JP.CMLiussss.net`
- `ProxyIP.HK.CMLiussss.net`
- `ProxyIP.KR.CMLiussss.net`
- `ProxyIP.DE.tp2024.CMLiussss.net`
- `ProxyIP.Aliyun.CMLiussss.net`
- `ProxyIP.Oracle.CMLiussss.net`
- `ProxyIP.DigitalOcean.CMLiussss.net`
- `ProxyIP.Vultr.CMLiussss.net`
- `ProxyIP.Multacom.CMLiussss.net`
</details>

<details>
<summary><code><strong>「 Preferred IP TXT Addresses Provided by This Project 」</strong></code></summary>

- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/HKG.txt` Hong Kong
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/KHH.txt` Taiwan
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/SIN.txt` Singapore
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/NRT.txt` Tokyo
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/SEA.txt` Seattle
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/LHR.txt` London
</details>

# Supported Clients

- v2ray
- clash

# Future Plans

- Support sing-box

# Disclaimer

This disclaimer applies to the "edge-tunnel" project (hereinafter referred to as "this project") on GitHub, with the project link: `https://github.com/ImLTHQ/edge-tunnel`

**Purpose**

- This project is designed and developed for educational, research, and security testing purposes only.
- It aims to provide security researchers, academics, and technology enthusiasts with a tool to explore and practice network communication technologies.
- The purpose is solely as a proxy to hide the real IP, not as a tool to bypass firewalls.

**Legality**

- When downloading and using the code of this project, you must comply with the applicable laws and regulations of the user. The user is responsible for ensuring that their actions comply with the legal framework, regulations, and other relevant provisions in their region.

**Disclaimer**

- As the **secondary development author** of this project (hereinafter referred to as "the author"), I, **ImLTHQ**, emphasize that this project is only for legal, ethical, and educational purposes.
- The author does not endorse, support, or encourage any form of illegal use. If it is found that this project is used for any illegal or unethical activities, the author will strongly condemn it.
- The author is not responsible for any illegal activities carried out by any person or organization using the code of this project. Any consequences arising from the use of the code of this project shall be borne by the user.
- The author is not responsible for any direct or indirect damages that may be caused by the use of the code of this project.
- To avoid any unexpected consequences or legal risks, users should delete the code within 24 hours after using the code of this project.

By using the code of this project, the user understands and agrees to all the terms of this disclaimer. If the user does not agree to these terms, they should immediately stop using this project.

The author reserves the right to update this disclaimer at any time without prior notice. The latest version of the disclaimer will be published on the GitHub page of this project.

# Thanks
[shulng](https://github.com/shulng), [XIU2](https://github.com/XIU2), [zizifn](https://github.com/zizifn), [cmliu](https://github.com/cmliu), [x0uid](https://github.com/x0uid)
