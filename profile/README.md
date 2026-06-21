<p align="center">
  <strong>A R C I S</strong><br>
  <em>The citadel of agent capital</em>
</p>

<p align="center">
  Financial infrastructure for autonomous AI agents.<br>
  Yield-bearing vaults · Identity-aware credit · Revenue bonds<br>
  <a href="https://arcis.money">arcis.money</a> · <a href="https://arcis.money/dashboard">Dashboard</a>
</p>

---

### Protocol

| Component | Description |
|---|---|
| **Agent Vaults** | ERC-4626 yield-bearing vaults. Deposit USDC, receive raUSDC. Strategies compound yield. |
| **Agent Credit** | Identity-aware credit via ERC-8004 reputation tiers. Utilization-based rate oracle. |
| **Revenue Bonds** | Agents issue tokenized bonds. Humans buy yield. Smart contracts service debt. |
| **CUSTOS** | Autonomous keeper agent. 9 skills. Harvests yield, monitors loans, services debt, engages community. |

### Repositories

| Repo | What | npm / Links |
|---|---|---|
| [`core`](https://github.com/Arcis-Protocol/core) | 17 contracts, 116 tests, ERC-4626, subgraph | Audit-ready |
| [`sdk`](https://github.com/Arcis-Protocol/sdk) | TypeScript SDK — vault + credit + bonds | `@arcisprotocol/sdk` |
| [`mcp`](https://github.com/Arcis-Protocol/mcp) | MCP server — 3 modes (local, HTTP, Vercel) | `@arcisprotocol/mcp` |
| [`custos`](https://github.com/Arcis-Protocol/custos) | Keeper agent — 4 keeper + 5 social skills | [README](https://github.com/Arcis-Protocol/custos) |
| [`cli`](https://github.com/Arcis-Protocol/cli) | Terminal TUI — vault, credit, bonds, MCP, CUSTOS | 12 commands |
| [`app`](https://github.com/Arcis-Protocol/app) | Landing + dashboard — arcis.money | 4 tabs |
| [`docs`](https://github.com/Arcis-Protocol/docs) | ATI v1.1, integration guide, SDK examples | 10 frameworks |
| [`monitor`](https://github.com/Arcis-Protocol/monitor) | Passive on-chain monitoring | Superseded by CUSTOS |

### ATI Standard

```
deposit(uint256 amount)  → uint256 shares
withdraw(uint256 shares) → uint256 amount
balance(address agent)   → uint256 value
```

Three functions. Any agent framework. The citadel has no gatekeepers.

### Security

- Emergency withdrawal (works when paused)
- 24-hour strategy addition timelock
- Withdrawal fee ramp (0.1% within 24h — flash loan protection)
- Per-agent deposit caps
- Utilization-based rate oracle (auto-adjusting interest rates)
- Full ERC-4626 view compatibility
- Zero `require()` — all custom errors
- 116/116 tests passing

---

<p align="center">
  <a href="https://x.com/ArcisProtocol">X</a> ·
  <a href="https://t.me/arcisprotocol">Telegram</a> ·
  <a href="https://github.com/Arcis-Protocol">GitHub</a> ·
  Base Sepolia
</p>
