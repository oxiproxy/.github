# OxiProxy

基于 Rust 的高性能内网穿透工具

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Rust](https://img.shields.io/badge/Rust-2021_Edition-orange.svg)](https://www.rust-lang.org/)
[![QUIC](https://img.shields.io/badge/Protocol-QUIC%2FKCP-blue.svg)](https://quicwg.org/)

OxiProxy 是一个现代化的内网穿透解决方案，采用 **Rust + QUIC/KCP + React** 技术栈，提供三层架构（Controller + Node + Client）的高性能反向代理服务。

## 特性

- **高性能** — 基于 Rust + QUIC/KCP 协议，低延迟、高并发
- **安全可靠** — TLS 加密传输，Token/JWT 认证机制
- **三层架构** — Controller + Node + Client 灵活部署
- **跨平台** — 支持 Linux、Windows、macOS（amd64/arm64）
- **可视化管理** — React 19 + shadcn/ui 构建的 Web 管理界面
- **多用户支持** — 多用户、多节点、多客户端、多隧道管理，支持订阅套餐与流量配额

## 架构

```text
Dashboard (React) ──HTTP/REST──▶ Controller (Axum + SQLite)
                                      │
                           gRPC Stream ├──▶ Node (QUIC/KCP)
                                      │          │
本地服务 ◀──TCP/UDP── Client ◀──gRPC──┘       公网服务
```

## 参与贡献

欢迎提交 Issue 和 Pull Request！

- **仓库**：[oxiproxy/oxiproxy](https://github.com/oxiproxy/oxiproxy)
- **Issues**：[反馈问题或提出建议](https://github.com/oxiproxy/oxiproxy/issues)
- **文档**：查看仓库 README 获取完整的安装和使用教程
