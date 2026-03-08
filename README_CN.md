<!-- markdownlint-disable MD041 -->
<div align="center">
  <h1>AIAP Store</h1>
  <p><b>AIAP 程序官方市场 — 发现、发布和分发 AI 能力包。</b></p>
  <p>
    <a href="https://aiap.dev"><img src="https://img.shields.io/badge/Protocol-AIAP_V1.0.0-brightgreen.svg" alt="AIAP V1.0.0" /></a>
    <a href="https://aiap.store"><img src="https://img.shields.io/badge/docs-aiap.store-blue.svg" alt="文档" /></a>
  </p>
  <p>
    English | <a href="README.md">English</a>
  </p>
</div>

## 什么是 AIAP Store？

AIAP Store 是 **AIAP 程序**的中央分发平台——遵循 [AIAP 协议](https://aiap.dev) 的 AI 能力包。它对于 AI 程序的意义，就如同 npm 之于 JavaScript 包，Docker Hub 之于容器镜像。

Store 上的每个程序均经过：

- **结构验证** — 通过 AIAP 协议合规性校验
- **质量评分** — ThreeDimTest 三维测试评估（正确性、内在质量、细节）
- **许可证声明** — 必须符合 PL25 规则，提供 SPDX 合规的 `license` 字段
- **治理签名** — SHA-256 governance hash 确保完整性可验证

---

## 生态系统

AIAP Store 是三层治理链的分发层：

```
aisop.dev   (种子层)   — 定义 .aisop.json 格式规范
aiap.dev    (权威层)   — 定义治理规则和质量标准
soulbot.dev (执行层)   — 执行 AIAP 程序的参考运行时
            ↓
aiap-store  (分发层)   — AIAP 程序的发现与分发市场
```

---

## 什么是 AIAP 程序？

AIAP 程序（`*_aiap/`）是结构化的 AI 能力包：

```
my_program_aiap/
├── AIAP.md            # 治理合约（声明身份、工具、信任级别、许可证）
├── main.aisop.json    # 带 mermaid 执行流程的程序入口
└── module.aisop.json  # 功能模块
```

程序通过 [AIAP Creator](https://soulbot.dev) 创建，在 [SoulBot](https://soulbot.dev) 运行时上执行。

---

## 上架要求

在 AIAP Store 发布程序，需满足以下条件：

| 要求 | 规则 | 说明 |
|------|------|------|
| 协议合规 | MF1 | 有效的 `AIAP.md` 治理合约 |
| 质量门槛 | ThreeDimTest | 达到最低通过分数 |
| 许可证声明 | PL25 | 每个程序必须在 `AIAP.md` 中声明自己的许可证，Store 平台不强制统一许可证 |
| 治理哈希 | MF15 | SHA-256 完整性验证 |
| 信任级别声明 | T1-T4 | 声明适当的权限边界 |

---

## 相关项目

| 项目 | 说明 | 链接 |
|------|------|------|
| **AIAP 协议** | 治理所有 AIAP 程序的开放标准 | [aiap.dev](https://aiap.dev) |
| **SoulBot** | AI Agent 框架 — 运行和创建 AIAP 程序 | [soulbot.dev](https://soulbot.dev) |
| **AIAP Creator** | 生成和验证 AIAP 程序的工具 | 已集成在 SoulBot 中 |

---

## 开发状态

AIAP Store 正在开发中。关注本仓库以获取上线通知。

- [ ] Store API 规范
- [ ] 程序提交门户
- [ ] 质量门禁 CI/CD 流水线
- [ ] 搜索与发现界面
- [ ] 作者认证系统

---

## 许可证

AIAP Store 是一个分发平台。**每个 AIAP 程序携带自己的许可证**，通过 `AIAP.md` 治理合约中的 `license` 字段声明（规则 PL25）。Store 平台本身不对托管的程序强制施加任何许可证。

---

对齐：人类主权与福祉。版本：AIAP V1.0.0。www.aiap.dev
