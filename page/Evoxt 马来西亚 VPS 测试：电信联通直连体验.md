# Evoxt 马来西亚 VPS 测试：电信联通直连体验

支持多种支付方式，包括支付宝、PayPal 和信用卡，为用户提供灵活便捷的购买选择。本文将详细测评 Evoxt 马来西亚 VPS 的性能、网络延迟、流媒体解锁情况及路由表现，帮助您全面了解其服务质量。

## 测评套餐概览

以下是本次测试所选用的 Evoxt 马来西亚 VPS 入门套餐 VM-0.5 的配置详情：

- **核心**: 1 vCore  
- **内存**: 512 MB RAM  
- **存储**: 5 GB Storage  
- **备份**: 每周备份  
- **价格**: $2.99/月  

这款套餐适合轻量级应用或个人测试使用，性价比颇高。

## 测试 IP 与 Looking Glass

测试使用的 IP 地址如下：  
- **IPv4**: 166.88.194.175  
- **IPv6**: 2400:8d60:5::1:203c:6a2a  

这些 IP 可用于自行验证网络连通性和性能。

## 流媒体解锁测试

以下是基于 Evoxt 马来西亚 VPS 的 IPv4 和 IPv6 地址的流媒体解锁情况，数据清晰展示其在多平台上的表现：

### IPv4 解锁结果

网络: Evoxt Enterprise (166.88.*.*)
Dazn: Yes (Region: MY)  
Disney+: No (IP Banned By Disney+)  
Netflix: Originals Only  
YouTube Premium: Yes (Region: MY)  
Amazon Prime Video: Yes (Region: MY)  
TVBAnywhere+: Yes  
Spotify Registration: Yes (Region: MY)  
Instagram Licensed Audio: No  
YouTube CDN: Kuala Lumpur  
Netflix Preferred CDN: Singapore  
ChatGPT: Yes  
Google Gemini: Yes (Region: MYS)  
Steam Currency: MYR  
Reddit: No

### IPv6 解锁结果

网络: Evoxt Enterprise (2400:8d60:5:*:*)
Dazn: IPv6 Not Supported  
Disney+: IPv6 Not Supported  
Netflix: Originals Only  
YouTube Premium: Yes (Region: MY)  
Amazon Prime Video: IPv6 Not Supported  
TVBAnywhere+: IPv6 Not Supported  
Spotify Registration: Yes (Region: MY)  
Instagram Licensed Audio: No  
YouTube CDN: Kuala Lumpur  
Netflix Preferred CDN: Singapore  
ChatGPT: Failed (Network Connection)  
Google Gemini: Yes (Region: MYS)  
Steam Currency: IPv6 Not Supported  
Reddit: IPv6 Not Supported

从结果来看，IPv4 在流媒体解锁方面表现更优，支持多种服务，而 IPv6 受限于协议兼容性，解锁能力较弱。

👉 [2025年最新 Evoxt 优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## TCP 回程路由测试

以下是针对不同网络（如上海电信、移动、联通及教育网）的回程路由测试结果，反映 Evoxt VPS 的网络连接质量：

### 上海电信路由

1   166.88.194.1    AS149440    美国 加利福尼亚州 圣克拉拉  evoxt.com    0.15 ms  
2   184.104.219.160 AS6939     马来西亚 吉隆坡 he.net               1.25 ms  
5   103.16.102.160  AS23764    新加坡 chinatelecomglobal.com       7.81 ms  
6   203.22.177.9    CTG-CN     中国 香港 电信                     43.09 ms  
8   59.43.247.233   CN2-Global 中国 上海 chinatelecom.cn       63.76 ms  
13  58.32.32.1      AS4812     中国 上海 长宁区 chinatelecom.cn    66.74 ms

### 上海移动路由

1   166.88.194.1    AS149440    美国 加利福尼亚州 圣克拉拉  evoxt.com    0.38 ms  
9   223.120.2.49    AS58453     中国 香港 cmi.chinamobile.com       39.28 ms  
11  221.183.89.170  AS9808      中国 上海 chinamobileltd.com       188.43 ms  
18  61.152.71.38    AS4812      中国 上海 普陀区 chinatelecom.cn    74.02 ms

### 上海联通路由

1   166.88.194.1    AS149440    美国 加利福尼亚州 圣克拉拉  evoxt.com    0.34 ms  
10  223.120.3.182   AS58453     中国 上海 cmi.chinamobile.com      221.77 ms  
18  112.65.63.1     AS17621     中国 上海 普陀区 chinaunicom.cn    177.73 ms

### 教育网路由

1   166.88.194.1    AS149440    美国 加利福尼亚州 圣克拉拉  evoxt.com    0.30 ms  
2   184.104.219.160 AS6939      马来西亚 吉隆坡 he.net              1.07 ms  
6   123.255.91.118  AS4538      中国 香港 edu.cn                   41.96 ms  
18  101.6.15.130    AS4538      中国 北京 海淀区 edu.cn           71.41 ms

电信和教育网的路由延迟较低，表现出色；移动和联通延迟稍高，但仍可满足日常需求。

## IPv6 路由表现

IPv6 路由因地区差异较大，建议用户根据实际网络环境自行测试，以获得更准确的结果。

## 网络速度与延迟测试

以下是 Evoxt 马来西亚 VPS 的速度和延迟表现：

Node Name       Upload Speed   Download Speed   Latency  
Speedtest.net   906.59 Mbps    882.00 Mbps      7.29 ms  
Singapore SG    907.31 Mbps    872.27 Mbps      9.07 ms  
Tokyo JP        703.77 Mbps    82.90 Mbps       101.76 ms  
USA US          252.01 Mbps    501.03 Mbps      280.52 ms  
DE DE           468.28 Mbps    346.42 Mbps      157.36 ms  
WuXi CU         3.27 Mbps      571.51 Mbps      130.46 ms

测试显示，Evoxt VPS 在东南亚地区（如新加坡）的速度和延迟表现尤为优异，适合需要低延迟和高带宽的用户。

## 总结

Evoxt 马来西亚 VPS 凭借电信和联通直连的优势，结合高性价比的套餐配置，在网络速度、流媒体解锁和路由表现上均有不俗表现。无论是个人测试还是轻量级应用，这款 VPS 都是值得考虑的选择。