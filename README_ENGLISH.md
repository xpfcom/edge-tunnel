# edge-tunnel

[简体中文](https://github.com/ImLTHQ/edge-tunnel/blob/main/README.md) | English

This is a script based on the CF platform.

I am a beginner, any code issues are welcome to be pointed out.

Please leave a star before you go!
[![Stargazers over time](https://starchart.cc/ImLTHQ/edge-tunnel.svg?variant=adaptive)](https://starchart.cc/ImLTHQ/edge-tunnel)

# Usage

Please register a `GitHub` and `Cloudflare` (hereinafter referred to as CF) account first.

- Fork this project on GitHub first.
- In the CF console, select `Workers`.
- Click `Create`, choose either `Workers` or `Pages`.
- Click `Connect to Git`, select the `edge-tunnel` project, and modify the `Project name`.
- Add `Variables` according to the `Variable Description` below.
- Click `Save and Deploy`.
- It is not immediately available after deployment, it takes about 10 minutes to wait.
- Import the subscription address `https://your_domain/subscription_path` into your Clash/V2ray client.

<details>
<summary><code><strong>「 Recommended actions after deployment 」</strong></code></summary>

Set up Github Action

- Go to your Forked repository
- Click the `green button` in the `Actions` tab.
- Select `Sync upstream`
- Click `Enable workflow`
- This is to keep your repository up-to-date with the author's synchronization.
</details>

<details>
<summary><code><strong>「 Bind a custom domain (optional) 」</strong></code></summary>

CF connects to your domain:

- Go to `Account Home`, select `Domain`, enter your domain name, click `Continue`.
- Select a plan according to your needs (the free one is enough), click `Continue`, click `Continue to activate`, click `Confirm`.
- According to CF's requirements, return to your domain service provider and replace your current DNS server with the CF DNS server.

Pages bind custom domain

- Click the `Custom Domain` tab of the Pages console, click `Set up a custom domain`.
- Enter the domain name.
- Click `Continue`, click `Activate domain`.
</details>

# Variable Description

| Variable Name | Example | Remarks |
|-|-|-|
| SUB_PATH | `sub` | Subscription path |
| SUB_UUID | `550e8400-e29b-41d4-a716-446655440000` | UUID for verification |
| TXT_URL | `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/HKG.txt` | Preferred IP TXT address. Supports multiple addresses separated by newlines. Format: address:port#node_name. Default port is 443 if not specified. Default node name is used if not specified. |
| SUB_NAME | `节点` | Default node name |
| PROXY_IP | `ts.hpc.tw:443` | Reverse proxy IP |
| SOCKS5_GLOBAL | `ture`,`false` | Enable SOCKS5 global reverse proxy |
| SOCKS5 | `username:password@address:port` | SOCKS5 |
| FAKE_WEB | `baidu.com` | The fake web page of the root path |

<details>
<summary><code><strong>「 More ProxyIP 」</strong></code></summary>

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
<summary><code><strong>「 Preferred TXT address provided by this project 」</strong></code></summary>

- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/HKG.txt` Hong Kong
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/KHH.txt` Taiwan
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/SIN.txt` Singapore
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/NRT.txt` Tokyo
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/SEA.txt` Seattle
- `https://raw.githubusercontent.com/ImLTHQ/edge-tunnel/main/SpeedTest/LHR.txt` London
</details>

# Adapted Clients

- v2ray
- clash

# Future Plans

- Support sing-box

# Disclaimer

This disclaimer applies to the "edge-tunnel" project (hereinafter referred to as "this project") on GitHub, with the project link: `https://github.com/ImLTHQ/edge-tunnel`

**Purpose**

- This project is designed and developed for educational, research, and security testing purposes only.
- It aims to provide a tool for security researchers, academics, and technology enthusiasts to explore and practice network communication technologies.
- Its purpose is solely as a proxy to hide the real IP, not as a tool to bypass firewalls.

**Legality**

- When downloading and using the code of this project, you must abide by the laws and regulations applicable to the user. The user is responsible for ensuring that their behavior complies with the legal framework, rules and regulations, and other relevant provisions of the region where they are located.

**Disclaimer**

- As the **secondary development author** (hereinafter referred to as "the author") of this project, I **ImLTHQ** emphasize that this project is only used for legal, ethical, and educational purposes.
- The author does not endorse, support, or encourage any form of illegal use. If it is found that this project is used for any illegal or unethical activities, the author will strongly condemn it.
- The author is not responsible for any illegal activities carried out by any person or organization using the code of this project. Any consequences arising from the use of the code of this project shall be borne by the user.
- The author is not responsible for any direct or indirect damages that may be caused by the use of the code of this project.
- To avoid any unexpected consequences or legal risks, the user should delete the code within 24 hours after using the code of this project.

By using the code of this project, the user understands and agrees to all the terms of this disclaimer. If the user does not agree to these terms, they should stop using this project immediately.

The author reserves the right to update this disclaimer at any time without prior notice. The latest version of the disclaimer will be published on the GitHub page of this project.

# Thanks
[shulng](https://github.com/shulng), [XIU2](https://github.com/XIU2), [zizifn](https://github.com/zizifn), [cmliu](https://github.com/cmliu), [x0uid](https://github.com/x0uid)
