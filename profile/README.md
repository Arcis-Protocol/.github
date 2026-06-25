<p align="center">
  <strong>A R C I S</strong><br>
  <em>The citadel of agent capital</em>
</p>

<p align="center">
  Financial infrastructure for autonomous AI agents.<br>
  Yield-bearing vaults · Identity-aware credit · Revenue bonds<br>
  <strong>Live on Base mainnet.</strong><br>
  <a href="https://arcis.money">arcis.money</a> · <a href="https://arcis.money/dashboard">Dashboard</a>
</p>

---

### Deployed Contracts (Base)

| Contract | Address |
|---|---|
| ArcisVault (raUSDC) | [`0x00325d9d...93e325a7`](https://basescan.org/address/0x00325d9da832b38179ed2f0dabd4062d93e325a7) |
| ATIRouter | [`0xeC3b7Daa...dB728F`](https://basescan.org/address/0xeC3b7Daa942C03651D55A4A01797498fA6dB728F) |
| StrategyAave | [`0x43626D61...F2F12a`](https://basescan.org/address/0x43626D6162Ccb12328B989BB228DaD2941F2F12a) |
| StrategyAllocator | [`0x7Fd5d7b4...6DD7A`](https://basescan.org/address/0x7Fd5d7b49694858FCf143E0039e83cDB0196DD7A) |

### Repositories

| Repo | What | npm / Links |
|---|---|---|
| [`core`](https://github.com/Arcis-Protocol/core) | 17 contracts, 116 tests, ERC-4626, Hardhat deploy | Audit-ready |
| [`sdk`](https://github.com/Arcis-Protocol/sdk) | TypeScript SDK — vault + credit + bonds | `@arcisprotocol/sdk` |
| [`mcp`](https://github.com/Arcis-Protocol/mcp) | MCP server — 3 modes (local, HTTP, Vercel) | `@arcisprotocol/mcp` |
| [`custos`](https://github.com/Arcis-Protocol/custos) | CUSTOS keeper — 4 keeper + 5 social skills | [@custos0x](https://x.com/custos0x) |
| [`cli`](https://github.com/Arcis-Protocol/cli) | Terminal TUI — 12 commands | Base mainnet |
| [`app`](https://github.com/Arcis-Protocol/app) | Landing + dashboard — arcis.money | 4 tabs |
| [`docs`](https://github.com/Arcis-Protocol/docs) | ATI v1.1, integration guide, SDK examples | 10 frameworks |
| [`monitor`](https://github.com/Arcis-Protocol/monitor) | Passive monitoring | Superseded by CUSTOS |

### ATI Standard

```
deposit(uint256 amount)  → uint256 shares
withdraw(uint256 shares) → uint256 amount
balance(address agent)   → uint256 value
```

### Security

Emergency withdrawal (works when paused) · 24h strategy timelock · 0.1% early withdrawal fee · Per-agent deposit caps · Utilization-based rate oracle · ERC-4626 compatible · Zero `require()` · 116 tests

---

<p align="center">
  <a href="https://x.com/ArcisProtocol">X</a> ·
  <a href="https://x.com/custos0x">CUSTOS</a> ·
  <a href="https://t.me/arcisprotocol">Telegram</a> ·
  <a href="https://github.com/Arcis-Protocol">GitHub</a> ·
  Base Mainnet
</p>
