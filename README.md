# Cloudflare-workers/pages Proxy Script

### This project only supports localized deployment

### All configurations in this project are edited locally, without using third-party external links like subscription managers or subscription converters, so there's no need to worry about node subscriptions being viewed by external link authors.

--------------------------------

## Script Features:

#### **For Lazy Beginners!** Default nodes are all official CF IPs, no need to frequently update subscriptions to get client-preferred IPs.

#### To reduce additional costs for beginners, this project does not recommend using custom domains, but you can if you must.

#### **Workers Method:** Supports vless+ws+tls, trojan+ws+tls, vless+ws, trojan+ws proxy nodes.

#### **Pages Method:** Supports vless+ws+tls, trojan+ws+tls proxy nodes.

#### Supports single node links, aggregated universal node subscriptions, sing-box node subscriptions, and clash node subscriptions.

#### Although only the obfuscated version is available, variables must be used only when modifying uuid/password.

-------------------------------------------------------------

### Communication Platforms: [Yongge's Blog](https://ygkkk.blogspot.com), [Yongge's YouTube Channel](https://www.youtube.com/@ygkkk), [Yongge's Telegram Group](https://t.me/+jZHc6-A-1QQ5ZGVl), [Yongge's Telegram Channel](https://t.me/+DkC9ZZUgEFQzMTZl)

--------------------------------

### Recommended for beginners to watch the following two introductory video tutorials:

[CF vless/trojan Free Node Obfuscation Era Arrives: Detailed Update Instructions After Workers/Pages Code Obfuscation; Summary of 1101 Error; Welfare Plan: Yongge Self-Built Multiple Proxy IPs for Everyone to Use](https://youtu.be/QSFaP5EVI04)

[CF vless/trojan Permanent Free Nodes (Please Replace the Code Content in the Video with Obfuscated Code): No Need for Custom Domains, Quick Start Guide; Free Client Setup Instructions for All Platforms; Exclusive Explanation of Preferred IP and Proxy IP Significance; One-Click Generation of Preferred Official IPs for the US, Hong Kong, and Europe](https://youtu.be/WwAeLyEz6jY)

---------------------------------------------

## One: CF Vless Node Configurable Variables

| Variable Purpose | Variable Name | Variable Value Requirements | Default Value | Variable Requirement |
| :--- | :--- | :--- | :--- | :--- |
| 1. Required UUID | uuid (lowercase letters) | Must conform to UUID format | Default UUID: 86c50e3a-5b87-49dd-bd20-03c7f2735e40 | Recommended |
| 2. Global Node Can Access CF Websites | proxyip (lowercase letters) | Port 443: IPv4 address, [IPv6 address], domain name. Non-443 port: IPv4 address:port, [IPv6 address]:port, domain name:port | Default proxyip domain: ts.hpc.tw | Optional |
| 3. Subscription Node: Preferred IP | ip1 to ip13, 13 in total | CF Official IP, CF Reverse Proxy IP, CF Preferred Domain | CF Official Different Region Visa Domains | Optional |
| 4. Subscription Node: Preferred IP Corresponding Port | pt1 to pt13, 13 in total | CF 13 Standard Ports, Reverse Proxy IP Corresponding Arbitrary Port | CF 13 Standard Ports | Optional |

---------------------------------

## Two: CF Trojan Node Configurable Variables

| Variable Purpose | Variable Name | Variable Value Requirements | Default Value | Variable Requirement |
| :--- | :--- | :--- | :--- | :--- |
| 1. Required Password | pswd (lowercase letters) | Recommended to use alphanumeric characters | Default Password: trojan | Recommended |
| 2. Global Node Can Access CF Websites | proxyip (lowercase letters) | Port 443: IPv4 address, [IPv6 address], domain name. Non-443 port: IPv4 address:port, [IPv6 address]:port, domain name:port | Default proxyip domain: ts.hpc.tw | Optional |
| 3. Subscription Node: Preferred IP | ip1 to ip13, 13 in total | CF Official IP, CF Reverse Proxy IP, CF Preferred Domain | CF Official Different Region Visa Domains | Optional |
| 4. Subscription Node: Preferred IP Corresponding Port | pt1 to pt13, 13 in total | CF 13 Standard Ports, Reverse Proxy IP Corresponding Arbitrary Port | CF 13 Standard Ports | Optional |

#### **Special Attention to Subscription Node IP and Port Variables (3 and 4) [Beginners Can Ignore Variables (3 and 4), Use Defaults]**

0. Since only obfuscated code can be used now, direct file modifications are not possible, only variables can be used.

1. **Remember:** Only when you must use a subscription client and want to change the preferred IP, you need to set variables ip1 to ip13, pt1 to pt13.

2. ip1 to ip7, pt1 to pt7, in the subscription share link, only support 80 series ports with TLS disabled nodes.

3. ip8 to ip13, pt8 to pt13, in the subscription share link, only support 443 series ports with TLS enabled nodes.

4. When setting official IPs, no need to set ports (13 CF standard ports are already set by default); when setting reverse proxy IPs, TLS must be enabled/disabled separately, and port variables must also be set.

5. For setting subscription node variables, please refer to this [video tutorial](https://youtu.be/8s-ELRuFaeE?si=MjhcKbt20d2Q2eqp&t=447).

---------------------------------

## Three: Custom proxyip

Although the script comes with other bigwigs' proxyip by default, it also supports custom proxyip.

Supports three methods: IPv4, IPv6, and domain name (when the port is 443, you can omit the :port).

1. **Global Node Variable Form (Already Explained in Sections One and Two):**

| proxyip Port | IPv4 Form | IPv6 Form | Domain Form |
| :--- | :--- | :--- | :--- |
| 443 Port | IPv4 Address | [IPv6 Address] | Domain Name |
| Non-443 Port | IPv4 Address:Port | [IPv6 Address]:Port | Domain Name:Port |

2. **Single Node Path Form:**

| proxyip Port | IPv4 Form | IPv6 Form | Domain Form |
| :--- | :--- | :--- | :--- |
| 443 Port | /pyip=IPv4 Address | /pyip=[IPv6 Address] | /pyip=Domain Name |
| Non-443 Port | /pyip=IPv4 Address:Port | /pyip=[IPv6 Address]:Port | /pyip=Domain Name:Port |

**Notes:**

1. **Single Node Path Change proxyip:** Only affects the currently setting single node, does not affect other single nodes or subscription nodes' proxyip.

2. **Global Node Change proxyip:** Affects all nodes without a path proxyip set.

3. When the node's path contains the ```/pyip=```

---------------------------------...

Citations:
[1] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/2716304/e05e91c9-60f9-4413-b666-412535818ccd/chinese.md
[2] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/2716304/fdedf166-9ff1-444c-a7e7-2753cf9a5ea6/paste.txt
[3] https://ppl-ai-file-upload.s3.amazonaws.com/web/direct-files/2716304/01299947-25cf-4ffd-bd71-67f4bf31fe38/paste-2.txt

## Four: No need for socks5! Easily create your own proxyip and any port reverse proxy IP for 80/443 systems using the reality protocol

### 1. For Serv00:

Modified from Serv00|ct8 Laowang's sing-box installation script, supporting one-click setup for three protocols: vless-reality, vmess-ws(argo), and hysteria2.

Mainly adds default support for CF vless/trojan node proxyip and non-standard port optimized reverse proxy IP functionality for the reality protocol.

For detailed setup video tutorial, please click [Serv00's most comprehensive proxy script](https://youtu.be/2VF9D6z2z7w)

One-click script for Serv00:

```bash
bash <(curl -Ls https://raw.githubusercontent.com/yonggekkk/Cloudflare_vless_trojan/main/serv00_proxyip.sh)
```

Script interface preview:

0bfd865cba72ccda1b3f34c7ee89fe9

Multi-account process keep-alive script is now supported. Place the kp.sh file on a third-party VPS server and modify the parameters inside for automatic scheduled running to keep nodes alive.

Serv00 keep-alive script, default nano editing mode. After adding parameters, run ```bash kp.sh```

```bash
curl -sSL https://raw.githubusercontent.com/yonggekkk/Cloudflare_vless_trojan/main/kp.sh -o kp.sh && chmod +x kp.sh && nano kp.sh
```

### 2. For VPS:

It's recommended to use pure IPv6 VPS that is close to China, cheap, and has high traffic allowance for setup. Try to avoid using IPv4 as it's likely to be scanned by others for reverse proxy IPs, becoming their public or paid reverse proxy IP pool. If you must use IPv4, please regularly monitor your VPS traffic, as using proxyip and client-optimized IPs will consume VPS traffic.

Recommended scripts for setting up proxyip and reverse proxy IP: [x-ui-yg script](https://github.com/yonggekkk/x-ui-yg), [sing-box-yg script](https://github.com/yonggekkk/sing-box-yg)

For related operations, please watch [Advanced Video Tutorial 1](https://youtu.be/QOnMVULADko) and [Advanced Video Tutorial 2](https://youtu.be/CVZStM0t8BA)

### 3. Four possible scenarios (recommended in TLS node environment):

Scenario 1: Only for client-optimized IP, i.e., CF node accessing non-CF websites will have the same IP location as the VPS region, while accessing CF websites will depend on the proxyip.

Scenario 2: Only for proxyip, i.e., CF node accessing CF websites will have the same IP location as the VPS region, while accessing non-CF websites will depend on the client-optimized IP.

Scenario 3: For both client-optimized IP and proxyip, i.e., CF node accessing both CF and non-CF websites will have IP locations matching the VPS region.

Scenario 4: By installing WARP global dual-stack V4+V6 functionality on VPS, either the client-optimized IP for non-CF websites (104.28.../2a09:...) or the proxyip for CF websites (104.28.../2a09:...) will show fixed or WARP unlocking effects.

## Five: View configuration information and sharing links

CF Vless: Enter https:// workers domain or pages domain or custom domain /custom uuid in the address bar

CF Trojan: Enter https:// workers domain or pages domain or custom domain /custom password in the address bar

Note:

1. If workers domain, pages domain, or custom domain are blocked, you must use a proxy to open them.
2. When using a custom domain, the configuration information and sharing links under the original workers domain or pages domain are still valid.

## Six: Optimized IP application

If you don't need the highest speed daily or country selection, you can use the default CF official IP or domain without changing.

Recommended easy-to-remember CF official IPs for lazy users (all IP locations are in the US, supporting 13 standard port switches), called "Immortal IPs at the Forefront":

104.16.0.0
104.17.0.0
104.18.0.0
104.19.0.0
104.20.0.0
104.21.0.0
104.22.0.0
104.24.0.0
104.25.0.0
104.26.0.0
104.27.0.0
172.66.0.0
172.67.0.0
162.159.0.0
2606:4700:: (requires IPv6 environment)

You can use IPs or domains shared by others by modifying configuration variables, or optimize locally. Refer to video tutorials for related optimization applications and scripts.

Recommended local computer-side optimization projects (can be downloaded directly from the code area above):

1. CDN Optimized Domain V23.8.18 (Computer Win64)
2. CF Optimized Reverse Proxy IP (Computer version, with speed test)
3. CF Optimized Official IP (US, Asia, Europe three regions, non-interactive computer version! Highly recommended! Click [video tutorial](https://youtu.be/6kKIzObEZ2c))
4. CF Optimized Official IP (Computer version, with speed test)

Note: When using load balancing or auto-selection for multiple CF nodes in the client, it's recommended that all applied nodes are from the same country/region to avoid IP jumping between different countries.

## Seven: Recommended clients

#### Benefits of enabling Fragment feature: Bypasses TLS blocking of blocked domains, allowing TLS nodes to support blocked domains like workers

#### Note: Custom domains or pages domains that are not blocked by TLS do not need to enable fragmentation to use TLS nodes

Currently supported platform clients are as follows (click the name to jump to the official download address):

1. Android: [v2rayNG](https://github.com/2dust/v2rayNG/tags), [Nekobox](https://github.com/maskedeken/NekoBoxForAndroid/tags), [Karing](https://github.com/KaringX/karing/tags), v2box

2. Windows: [v2rayN](https://github.com/2dust/v2rayN/tags), [Hiddify](https://github.com/hiddify/hiddify-next/tags), [Karing](https://github.com/KaringX/karing/tags)

3. iOS: Karing, Hiddify Proxy & VPN, Shadowrocket, Streisand, v2box

4. OpenWrt router: [homeproxy](https://github.com/kiddin9/openwrt-packages), recommended to use the system's built-in software library to find updates

Note: For other platform clients without fragmentation enabled, the 6 443-system TLS nodes of the workers domain are not available.

Note: Shadowrocket, v2box, v2rayn, v2rayng clients have a forced TLS enabling issue with trojan+ws, causing trojan+ws to not work. Also, clash subscriptions do not have trojan+ws nodes. Please note this.

For client usage issues, please watch [CF vless/trojan Permanent Free Node Tutorial (Six): Node Not Working, Where's the Problem? Multi-Platform Free Client Setup Guide and Pitfall Explanations](https://youtu.be/8E0l0nQWLxs)

### CF Video Tutorial Collection:

[CF workers Permanent Free vless Node Setup Tutorial (One): First demonstration of IP jumping phenomenon, decrypting two major node usage techniques, explaining pros and cons of optimized IP and optimized domain](https://youtu.be/9V9CQxmfwoA)

[CF workers Permanent Free vless Node Setup Tutorial (Two): Release of one-click script for optimized reverse proxy IP, pages deployment tutorial, multi-platform client setup instructions, exclusive discussion on CF free proxy sensitivity and security issues](https://youtu.be/McdRoLZeTqg)

[CF workers Permanent Free Trojan Node Setup Tutorial (Three): No need for custom domain, workers and pages two schemes to deploy optimized IP nodes; comparison summary of CF Trojan and CF Vless; how to view Trojan being identified](https://youtu.be/lmhhL8M1k0I)

Highly recommended: [CF vless/trojan Permanent Free Node Tutorial (Four): Interpreting the relationship and characteristics of optimized official IP, optimized reverse proxy IP, and optimized domain; the significance of ProxyIP](https://youtu.be/NaLd-orwFUE)

Highly recommended: [CF vless/trojan Permanent Free Node Tutorial (Five): No custom domain? No frequent IP optimization? No subscription generator? Summarizing the structural relationship diagram of CF nodes and domains](https://youtu.be/8s-ELRuFaeE)

Highly recommended: [CF vless/trojan Permanent Free Node Tutorial (Six): Node Not Working, Where's the Problem? Multi-Platform Free Client Setup Guide and Pitfall Explanations](https://youtu.be/8E0l0nQWLxs)

Advanced recommendation: [CF vless/trojan Permanent Free Node Final Tutorial (Seven): Web-exclusive demonstration of true "fixed IP", solving twitch, chatgpt client error issues; one-click self-made reverse proxy IP and ProxyIP; revealing the risk of your IP being scanned by others](https://youtu.be/QOnMVULADko)

Advanced recommendation: [CF vless/trojan Permanent Free Node Final Tutorial (Eight): Self-build all-port universal ProxyIP, simultaneously supporting client address optimization reverse proxy IP, final tutorial for self-building reverse proxy IP](https://youtu.be/CVZStM0t8BA)

[Live Stream Highlights: Four major features of CF workers vless free nodes, node disconnection and blocking issues](https://youtu.be/9OHGpWlfdJ0)

[ClouDNS Permanent Free Domain Final Tutorial: CF pages vless custom domain direct deployment](https://youtu.be/PN0BLANXh4I)

Beginner-friendly optimized IP application recommendation: [CF Optimized IP Liberation for Beginners Final Solution: One-click automatic generation of optimized official IPs for US, Hong Kong, Europe three regions, one-click universal for multiple platforms including computer WIN, Android, iOS](https://youtu.be/6kKIzObEZ2c)

Latest recommendation: [CF vless/trojan Free Node Obfuscation Era Arrives: Detailed setup instructions after workers/pages code obfuscation; 1101 error summary; Benefit plan: Yong Ge self-builds multiple ProxyIPs for everyone to use](https://youtu.be/QSFaP5EVI04)

## Optimized domain, optimized official IP + reverse proxy IP one-click script (run in local network environment using termux or ish):

1. For Android, please use the official termux project to download the client (Google Play Store version is not usable!): https://github.com/termux/termux-app/releases/tag/v0.118.1

After first installation, please install dependencies first: ```pkg upgrade```

2. For iPhone users, due to a bug in the latest version of ISH causing the script to freeze, please use ISH_1.2.2 version. You can install it with Trollstore and then downgrade, or follow other online tutorials for installing specific old IPA versions

After first installation, please install dependencies first: ```apk add curl bash```

### Script 1: CF-Optimized Official IP (default US, Asia, Europe three regions, highly recommended!!!), for Android and iOS phones and tablets:

```bash
curl -sSL https://raw.githubusercontent.com/yonggekkk/Cloudflare_vless_trojan/main/cf/cf.sh -o cf.sh && chmod +x cf.sh && bash cf.sh
```

### Script 2: CF-CDN Optimized Public Large Factory Domain Script, for iOS and Android phones and tablets:

```bash
curl -sSL https://gitlab.com/rwkgyg/CFwarp/raw/main/point/CFcdnym.sh -o CFcdnym.sh && chmod +x CFcdnym.sh && bash CFcdnym.sh
```

### Script 3: CF-Optimized Official IP + Reverse Proxy IP Two-in-One Script (with speed test), for iOS and Android phones and tablets:

```bash
curl -sSL https://gitlab.com/rwkgyg/CFwarp/raw/main/point/cfip.sh -o cfip.sh && chmod +x cfip.sh && bash cfip.sh
```

### Thank you for your star🌟 in the upper right corner

[Stargazers over time

### Code sources: [ca110us](https://github.com/ca110us/epeius), [emn178](https://github.com/emn178/js-sha256/blob/master/src/sha256.js), [3Kmfi6HP](https://github.com/3Kmfi6HP/EDtunnel), [badafans](https://github.com/badafans/Cloudflare-IP-SpeedTest), [XIU2](https://github.com/XIU2/CloudflareSpeedTest), [Laowang eooce](https://github.com/eooce/Sing-box/blob/test/sb_00.sh), [frankiejun](https://github.com/frankiejun/serv00-play/blob/main/start.sh)
