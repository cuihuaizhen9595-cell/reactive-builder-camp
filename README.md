# Reactive Builder Camp 学习笔记

记录 Reactive Omni 训练营的每日打卡、测试网练习和验证结果。本仓库以 2026-10-28 主网迁移后的 Omni 写法为准。

## 如何记录

- 每天把笔记保存在 `notes/YYYY-MM-DD.md`，可从 [打卡模板](notes/README.md) 复制。
- 后续练习源码可放 `src/`，测试可放 `test/`。
- 链上练习记录网络、测试结果和可公开的测试网交易哈希。钱包助记词、私钥、访问令牌以及带密钥的 RPC 地址仅保留在本地。

## 工具与网络

```powershell
forge --version
cast --version
```

练习使用独立测试账户。Ethereum Sepolia 的链 ID 是 `11155111`；Reactive Lasna 的链 ID 是 `5318007`，原生测试币为 `lREACT`。网络参数和测试币入口见 [Reactive Mainnet / Lasna Testnet](https://dev.reactive.network/reactive-mainnet#get-testnet-react)。

## Omni 参考

- [Reactive Contracts](https://dev.reactive.network/reactive-contracts)：`react()` 加 `onlySystem`，用 `SYSTEM.requestCallbackV_1_0` 请求回调。
- [Callback Contracts](https://dev.reactive.network/callback-contracts)：目标链回调同时校验代理与 Reactive 合约地址。
- [Economy](https://dev.reactive.network/economy)：两端分别检查余额、储备和欠费。
- [Omni Micro Demos](https://github.com/Reactive-Network/reactive-smart-contract-demos/tree/omni/src/micro-demos)：以 `omni` 分支为准。
