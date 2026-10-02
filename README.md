<div align="center">

# Arbitrage Inc Earn

[![CI](https://github.com/arbincept/arbitrage-inc-earn/actions/workflows/ci.yml/badge.svg)](https://github.com/arbincept/arbitrage-inc-earn/actions/workflows/ci.yml)

**Explore BNB Chain lending and liquid staking in one interface.**

Built and maintained by **[Luca Celebrano · @Lukecele](https://github.com/Lukecele)**, founder of [Arbitrage Inception](https://github.com/arbincept).

**[Open app](https://arbitrage-inc-earn.vercel.app)** · **[Star this repository](https://github.com/arbincept/arbitrage-inc-earn)** · **[Follow Lukecele](https://github.com/Lukecele)**

[Quick start](#quick-start) · [Contribute](#contribute) · [MIT license](LICENSE)

</div>

![Arbitrage Inc Earn vault explorer with lending and liquid-staking strategies](docs/live-vaults.png)

<sub>Application screenshot from this repository. Live data and available routes change over time.</sub>

## What you can explore

| Integration | Interface focus |
| :--- | :--- |
| **Venus Protocol** | BNB Chain lending markets. |
| **Lista DAO** | Liquid staking with slisBNB. |
| **Stader** | Liquid staking with BNBx. |
| **pSTAKE** | Liquid staking with stkBNB. |
| **KyberSwap** | Token quotes and route building for supported entry flows. |

Built with **Next.js, React, TypeScript, viem, and wagmi**. This is the dedicated Earn application linked from [Arb-Inc All-in-Dex](https://github.com/arbincept/Arb-Inc-All-in-Dex).

## Try it

1. Open the vault explorer and inspect the available strategies.
2. Choose a destination and review its required asset, displayed protocol data, and route estimate.
3. If you choose to proceed, connect a wallet and review each approval and transaction before signing.

Displayed rates and protocol availability can change. Wallet approvals, swaps, and deposits interact with third-party contracts; displayed yield is an estimate.

## Quick start

Use **Node.js 22+** and **npm**, matching the repository's CI toolchain.

```bash
git clone https://github.com/arbincept/arbitrage-inc-earn.git
cd arbitrage-inc-earn
npm install
npm run dev
```

Open [localhost:3000](http://localhost:3000).

### Project checks

```bash
npm run lint
npm run build
```

These are the checks configured in [CI](.github/workflows/ci.yml). There is no `npm test` script.

## Explore the implementation

| File | Start here for |
| :--- | :--- |
| [app/page.tsx](app/page.tsx) | Main application page. |
| [lib/kyberswap.ts](lib/kyberswap.ts) | Quotes, fee parameters, and route building. |
| [lib/abis.ts](lib/abis.ts) | Contract interface definitions. |
| [package.json](package.json) | Scripts and dependencies. |

The KyberSwap helper requests a `50` bps fee and defaults to `50` bps slippage tolerance. Review the returned quote and transaction details for the selected route.

## Deployment notes

The interface relies on external RPC and protocol APIs. Quotes, balances, and displayed rates depend on their availability. Keep network selection, contract addresses, allowances, and minimum output under review when adapting the code for your own deployment.

## Contribute

Reproducible bug reports, clearer documentation, and focused improvements are welcome. Start with an [issue](https://github.com/arbincept/arbitrage-inc-earn/issues) describing the behavior, environment, and expected result. Include the relevant checks with a pull request.

For sensitive reports, use the organization's [security policy](https://github.com/arbincept/.github/blob/main/SECURITY.md).

## More from Lukecele

This project is part of an independent ecosystem built by **[Luca Celebrano (@Lukecele)](https://github.com/Lukecele)**.

[Arb-Inc All-in-Dex](https://github.com/arbincept/Arb-Inc-All-in-Dex) · [Inception Flap Scanner](https://github.com/arbincept/inception-flap-scanner) · [BSC Arbitrage Scanner](https://github.com/arbincept/bsc-arbitrage-scanner)

If this project helps you, **[give it a star](https://github.com/arbincept/arbitrage-inc-earn)** and **[follow Lukecele](https://github.com/Lukecele)** for future builds. [Sponsorship](https://github.com/sponsors/Lukecele) helps support ongoing work.

[Telegram](https://t.me/ArbitrageInception) · [Updates on X](https://x.com/Arbitrageincept) · [MIT license](LICENSE)