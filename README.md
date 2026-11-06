# Super Adblock Test hostname probes for AdGuard Home

An **unofficial, static snapshot** of the hostname probes in [Super Adblock Test](https://superadblocktest.com/), formatted as a DNS blocklist for AdGuard Home. This repository is not affiliated with the test site.

## AdGuard Home subscription URL

```text
https://raw.githubusercontent.com/hdbp/superadblocktest-adguard-home/main/blocklist.txt
```

In AdGuard Home, open **Filters → DNS blocklists → Add blocklist → Add a custom list** and paste the URL above.

## Scope and limitations

- The source script was read on 2026-11-06: [adblock.js](https://superadblocktest.com/adblock.js?v=20260810-direct-run-1).
- It contained 482 probes. `blocklist.txt` contains 476 exact hostnames. Six path-specific probes cannot be represented precisely in DNS and are omitted from active rules.
- Browser cosmetic rules and URL-path rules are included only as comments; AdGuard Home ignores them.
- Blocking the entire list can interfere with sites and apps, especially consent, analytics, video, and affiliate services. Use it for testing and review the domains you actually want to block.
- This snapshot does **not** update automatically when the test site's probes change. Updates to this repository will appear at the same subscription URL.
- A high benchmark score does not prove that all real-world ads are blocked. Confirm that client queries reach AdGuard Home in its Query Log.
