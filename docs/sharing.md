# Sharing Arbitrage Inc Earn

## Introduction draft

Explore BNB Chain lending and liquid staking with Arbitrage Inc Earn, an open-source interface built by Luca Celebrano (@Lukecele), founder of Arbitrage Inception.

Use the vault explorer to compare the assets shown for Venus, Lista DAO (slisBNB), Stader (BNBx), and pSTAKE (stkBNB), then inspect the route estimate for your chosen entry flow. Browsing does not require a wallet; approvals and transactions require connecting a wallet and reviewing each signature request.

Displayed yields are estimates, not guaranteed returns. The current dashboard's APY labels are static values defined in the source, not live protocol-rate feeds. The KyberSwap helper requests a 50 bps fee and defaults to 50 bps slippage tolerance.

[Try the app](https://arbitrage-inc-earn.vercel.app) · [Star the repository](https://github.com/arbincept/arbitrage-inc-earn) · [Follow Lukecele](https://github.com/Lukecele)

This is a draft for the maintainer to publish.

## Social card

Editable source: [social-card.svg](social-card.svg).

- Canvas: 1280 × 640, with an opaque dark background for consistent display in light and dark themes.
- Text: “Arbitrage Inc Earn”, “Explore BNB Chain lending & liquid staking”, and “by Lukecele”.
- Provenance: the existing crossed-infinity mark from [Navbar.tsx](../components/Navbar.tsx); slate, emerald, and cyan colors from the interface. No new logo, third-party imagery, or simulated application screenshot.
- Export: render the SVG in a browser, draw it onto a 1280 × 640 canvas, and export as PNG. Check that the final PNG is under 1 MB before upload. Text uses system Arial/Helvetica/sans-serif, so font metrics may vary between environments.
- The PNG delivered with this change is a sharing graphic, not an application screenshot. Adding this SVG to Markdown does not configure GitHub's social preview.

GitHub recommends 1280 × 640 and an image under 1 MB. Upload the exported PNG in **Settings → General → Social preview → Edit → Upload an image**. See [GitHub's social preview documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/customizing-your-repositorys-social-media-preview).

## Existing screenshot

[Original vault explorer screenshot](live-vaults.png) is preserved unchanged from commit `42cd003e84d1ad15d628354a1956d7b9eaa9ccf7`, which introduced it as the live vault preview. It is already a narrow mobile capture. Cropping away the header would remove useful context and would not reveal additional strategies beyond the captured viewport. Rates visible in the image are historical interface labels; the image is not evidence of current protocol yields.

## Repository discovery settings

These are the requested editorial values, separate from the README and social preview:

| Setting | Requested value |
| :--- | :--- |
| Description | Open-source BNB Chain lending and liquid-staking interface for Venus, Lista DAO, Stader and pSTAKE. Built by Lukecele. |
| Website | https://arbitrage-inc-earn.vercel.app |
| Topics | `defi`, `bnb-chain`, `lending`, `liquid-staking`, `venus-protocol`, `lista-dao`, `stader`, `pstake`, `kyberswap`, `nextjs`, `typescript`, `viem`, `wagmi` |

On 2026-10-01, the repository API showed that the website already matched and all 13 requested topics were present among 20 existing topics. The description still differed. No settings were changed by this task because the available access did not permit repository administration.

A maintainer can use the gear beside **About** on the repository page to apply the description and exact topic list above, preserving the existing website. Topics meet GitHub's limit of 20, with at most 50 lowercase letters, digits, or hyphens per topic. See [GitHub's topic documentation](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics).

The [All-in-Dex Earn gateway](https://arbitrage-inc.exchange/vaults) links to this separate application. Both the gateway and the Earn homepage returned HTTP 200 when checked on 2026-10-01; this check did not exercise wallet or protocol operations.
