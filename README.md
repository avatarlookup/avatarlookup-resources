# AvatarLookup resources

Official technical resources, guides and developer articles for **AvatarLookup** — public avatar lookups and portrait attribute analysis.

- **Website:** https://avatarlookup.com
- **Blog:** https://avatarlookup.com/blog
- **API documentation:** https://avatarlookup.com/api-docs
- **Pricing:** https://avatarlookup.com/pricing

## What is in this repository

This repository is the public home for AvatarLookup technical writing that is published outside the website:

- **[Issues](../../issues)** — short technical notes on integration, result interpretation and operational practice.
- **[Discussions](../../discussions)** — longer announcements and product guidance under the *Announcements* category.

The canonical version of every product fact lives on the website. Where an article and the site disagree, the site wins.

## Official API example repositories

One repository per product, each with an OpenAPI contract, a machine-readable `product.json`, an `llms.txt` summary and runnable examples in seven languages.

| Product | Shape | Repository |
|---|---|---|
| [WhatsApp avatar analysis](https://github.com/avatarlookup/whatsapp-avatar-profile-api) | Realtime | `whatsapp-avatar-profile-api` |
| [Email avatar analysis](https://github.com/avatarlookup/email-avatar-profile-api) | Realtime | `email-avatar-profile-api` |
| [Image profile analysis](https://github.com/avatarlookup/image-profile-analysis-api) | Realtime | `image-profile-analysis-api` |
| [Email Bulk Avatar Check](https://github.com/avatarlookup/email-bulk-avatar-api) | Bulk (async) | `email-bulk-avatar-api` |
| [LINE Bulk Avatar Analysis](https://github.com/avatarlookup/line-bulk-profile-api) | Bulk (async) | `line-bulk-profile-api` |
| [MAX Bulk Number Profile](https://github.com/avatarlookup/max-bulk-profile-api) | Bulk (async) | `max-bulk-profile-api` |
| [Telegram Bulk Number Profile](https://github.com/avatarlookup/telegram-bulk-number-profile-api) | Bulk (async) | `telegram-bulk-number-profile-api` |
| [Telegram Bulk Username Profile](https://github.com/avatarlookup/telegram-bulk-username-profile-api) | Bulk (async) | `telegram-bulk-username-profile-api` |
| [Viber Bulk Number Profile](https://github.com/avatarlookup/viber-bulk-profile-api) | Bulk (async) | `viber-bulk-profile-api` |
| [WhatsApp Bulk Avatar Analysis](https://github.com/avatarlookup/whatsapp-bulk-avatar-api) | Bulk (async) | `whatsapp-bulk-avatar-api` |
| [Zalo Bulk Number Profile](https://github.com/avatarlookup/zalo-bulk-profile-api) | Bulk (async) | `zalo-bulk-profile-api` |

A **realtime** check answers inside the same HTTP response (`POST /api/v1/check`, or `POST /api/v1/batch-check` for up to 100 identifiers). A **bulk task** takes a file and answers later (`POST /api/v1/bulk-tasks`). They are separate endpoints and are not interchangeable.

## Responsible use

AvatarLookup results are **point-in-time signals**. A result describes what a provider reported at the moment of the check — it is not identity verification, not proof of ownership, and not permission to contact anyone. Use the API only for identifiers you are authorized to process, and comply with applicable privacy laws and platform terms.

Third-party trademarks belong to their respective owners; no affiliation or endorsement is implied.

---

*Maintained by AvatarLookup. Questions and integration problems: https://avatarlookup.com/contact*
