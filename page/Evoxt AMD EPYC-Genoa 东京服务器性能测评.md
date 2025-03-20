# Evoxt AMD EPYC-Genoa 东京服务器性能测评

## Evoxt 云服务器简介

Evoxt 成立于 2020 年，是一家致力于以高性价比提供优质虚拟专用服务器（VPS）的服务商，目标是打破云虚拟机行业普遍存在的高价低性能瓶颈。Evoxt 采用 KVM 虚拟化技术，结合企业级硬件，为用户提供卓越的性能与可靠性。其服务亮点包括：

- **虚拟机管理功能**：支持监控、IP 地址管理、防火墙设置、克隆、子账户管理、备份、VNC 控制和 API 接口。
- **安全保障**：提供隔离环境、三层防火墙、DDoS 防护以及每周自动异地备份。
- **全球覆盖**：数据中心遍布 14 个地区，包括东京、香港、大阪、洛杉矶、伦敦等地。

本文将聚焦于 Evoxt 在东京部署的 AMD EPYC-Genoa 处理器服务器，通过多项测试数据展示其性能表现。

## 硬件配置概览

以下是 Evoxt 东京服务器的硬件信息：

Architecture: x86_64
CPU(s): 1
Vendor ID: AuthenticAMD
Model name: AMD EPYC-Genoa Processor
CPU family: 25
Thread(s) per core: 1
Core(s) per socket: 1
Socket(s): 1
BogoMIPS: 7386.03
Hypervisor vendor: KVM
Virtualization type: full
Caches: L1d: 32 KiB, L1i: 32 KiB, L2: 1 MiB, L3: 32 MiB

核心关键词：**AMD EPYC-Genoa**、**KVM 虚拟化**、**东京服务器**。这台服务器搭载单核 AMD EPYC-Genoa 处理器，配备 1.9 GiB 内存和 19.6 GiB 存储空间，运行 Debian 12 系统，适合轻量级应用和测试场景。

## Yabs 性能测试

Yabs 测试展示了服务器的基础性能和磁盘、网络速度：

### 系统基本信息
- **处理器**：AMD EPYC-Genoa @ 3693.018 MHz
- **内存**：1.9 GiB
- **磁盘**：19.6 GiB
- **虚拟化**：KVM
- **操作系统**：Debian GNU/Linux 12

### 磁盘速度 (fio 测试)
| 块大小 | 读速 (IOPS)      | 写速 (IOPS)      | 总速 (IOPS)      |
|--------|------------------|------------------|------------------|
| 4k     | 123.62 MB/s (30.9k) | 123.95 MB/s (30.9k) | 247.58 MB/s (61.8k) |
| 64k    | 1.23 GB/s (19.3k)  | 1.24 GB/s (19.4k)  | 2.48 GB/s (38.8k)  |
| 512k   | 1.56 GB/s (3.0k)   | 1.64 GB/s (3.2k)   | 3.21 GB/s (6.2k)   |
| 1m     | 1.50 GB/s (1.4k)   | 1.60 GB/s (1.5k)   | 3.10 GB/s (3.0k)   |

磁盘性能表现出色，尤其在较大块大小下，总读写速度可达 3 GB/s 以上，适合高吞吐量任务。

### 网络速度 (iperf3 测试)
- **IPv4 下载速度**：最高 2.13 Gbits/sec（新加坡）
- **IPv4 上传速度**：最高 1.63 Gbits/sec（新加坡）
- **IPv6 下载速度**：最高 1.73 Gbits/sec（新加坡）
- **IPv6 上传速度**：最高 1.68 Gbits/sec（洛杉矶）

东京服务器网络表现优异，亚洲区域延迟低，跨洲连接稳定。👉 [2025年最新Evoxt优惠码和云服务器方案套餐整理汇总](https://bit.ly/evoxt)

## GeekBench 5 测试

GeekBench 5 结果显示：
- **单核分数**：1633
- **多核分数**：1677
- **处理器**：AMD EPYC-Genoa @ 3.69 GHz
- **内存**：1.92 GB

单核性能强劲，多核分数受限于单核配置，但整体表现适合计算密集型任务。

## UnixBench 测试

UnixBench 测试反映系统综合性能：
- **Dhrystone 2**：66822795.7 lps（指数 5726.0）
- **Whetstone**：11342.6 MWIPS（指数 2062.3）
- **文件复制 (1024 bufsize)**：1846454.2 KBps（指数 4662.8）
- **系统基准指数**：954.7

文件操作和计算能力突出，表明服务器在多种工作负载下均有良好表现。

## A Bench 测试

A Bench 测试提供更全面的性能数据：
- **I/O 平均速度**：552.3 MB/s
- **网络速度 (东京)**：下载 2509.79 Mbps，上传 2586.55 Mbps
- **延迟**：0.71 ms（Speedtest.net）

低延迟和高带宽使该服务器非常适合亚洲用户，尤其是日本本地应用场景。

## 流媒体解锁测试

### IPv4 结果
- **Netflix**：仅支持自制剧（区域：英国）
- **YouTube**：正常解锁（区域：日本，缓存节点：东京）
- **Disney+**：支持解锁

### IPv6 结果
- **Netflix**：无正常 IPv6 接入
- **YouTube**：不支持服务

流媒体解锁能力有限，IPv4 表现优于 IPv6，适合 YouTube 和 Disney+ 用户。

## IP 质量与安全性

- **ASN**：AS149440 Evoxt Enterprise
- **位置**：日本东京
- **威胁级别**：低
- **欺诈得分**：25（低）
- **用途**：数据中心/托管服务

IP 安全性较高，适合企业级应用和托管需求。

## 总结

Evoxt 东京服务器凭借 AMD EPYC-Genoa 处理器和 KVM 虚拟化技术，在磁盘速度、网络性能和计算能力上均表现出色，尤其适合亚洲用户的高性能需求。无论是轻量级网站托管还是流媒体应用，这款服务器都能提供稳定支持。欲了解更多优惠信息，可查看：[https://bit.ly/evoxt](https://bit.ly/evoxt)。