# DSC Manager v14: KDK-rules redesign (mockup)

A single-file HTML mockup. No build step, no server, no libraries.

## Run
1. Open `index.html` in Edge, Chrome or Firefox (double-click is enough).
2. Added DSCs and filters are kept in this browser (localStorage, keys start with `dscMgrV14.`).
3. To start again: **Mockup ▾ → Reset demo data**.

The Mockup menu (dashed button, top right) holds the demo-only aids: change notes, column filter plan, slow motion, reduced motion.

## What is in it
- Overview: four figure tiles, import banner, portal cards (GST, TDS, ITR, Others), renewals due. Every tile and card opens the rows behind it.
- All DSCs: grouped by client with [+] / [−] boxes, search with scope (client, PAN, holder, serial), portal, availability, status, issuer, token make and colour. Missing signatories appear as rows next to the certificates.
- Clients with No DSC: one row per missing signatory (client, portal, signatory, PAN, designation, Add DSC).
- Client details: side panel by portal (GST, TDS, ITR) and Others.
- Add DSC: manual entry or demo scan, grouped fields, typed dates (15/10/26, 151026, 15oct26), inline errors.
- Review scans: demo queue, opens the same form so values can be edited.

## Sample data
Unchanged from v13: 15 clients, 31 signatories, 25 DSCs. At the start 6 clients (9 signatories) are in Clients with No DSC and 3 DSCs are under Others.

## Keys
`/` search · `Ctrl+K` Tools · `Ctrl+\` keep panel open or fold · `Alt+L` slide panel out · `+` / `−` open or close a group · `Alt+Shift+↓/↑` expand or collapse all · `Esc` close.

## Limits
- Scan DSC is a demo. It never reads a USB token.
- Phones show the full app as cards (the KDK rule says status page only; the brief asked for working phones).
- Data lives in the browser only. There is no server.
