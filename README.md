# user-group-presentations

Slide decks from the DIDComm user group, published with GitHub Pages at
<https://wyvrn-cloud.github.io/user-group-presentations/>.

Each deck lives in its own directory as an `index.html`. The root
`index.html` is the landing page that lists them; add a deck there to make
it discoverable. Decks that aren't listed are still reachable by URL.

## Presentation order

Each talk is framed as "here's a way to approach the problem", built on the
DIDComm Messaging spec and its extensions. Where wyvrn comes up, it is an
experiment, not the subject.

| # | Deck | Status | Why this position |
|---|------|--------|-------------------|
| 1 | [Identity DID, Device DID](identity-vs-device-dids/) | **Next up** · listed | Per-device keys for one identity. Current focus. |
| 2 | [Catching Up a New Device](catching-up-a-new-device/) | Draft | Direct follow-on: what a newly enrolled device sees. |
| 3 | [Group Conversations on a Pairwise Protocol](group-conversations/) | Draft | Builds on the roster and fan-out ideas from 1–2. |
| 4 | [What a Mediator Actually Does](what-a-mediator-does/) | Draft | Routing foundations that 5–8 lean on. |
| 5 | [DIDComm over Bluetooth](didcomm-over-bluetooth/) | Draft | Local first, mediator as fallback. Needs 4. |
| 6 | [DIDComm in CBOR?](didcomm-in-cbor/) | Draft | Encoding size; motivated by 5's small packets. |
| 7 | [DIDComm on Small Devices](didcomm-on-small-devices/) | Draft | IoT; pulls together 4, 5 and 6. |
| 8 | [DIDComm Without a Network](didcomm-without-a-network/) | Draft | Supply chain and offline transports. |
| 9 | [Beyond Messages: Streaming and Broadcast](streaming-and-broadcast/) | Draft | Mostly open questions; best once the group has context. |
| 10 | [DIDComm and Post-Quantum Crypto](post-quantum-didcomm/) | Draft | Cross-cutting; touches everything above. |

`where-wyvrn-chat-stands/` is an older deck, left in place but not listed.

## Layout

- `identity-vs-device-dids/` and `where-wyvrn-chat-stands/` are fully
  self-contained (reveal.js core CSS inlined), so they also work when
  published as standalone artifacts.
- The drafts share `assets/deck.css` for their theme and load reveal.js
  6.0.2 (including its speaker-notes plugin) from jsDelivr. Press **S** in a
  draft to open speaker notes; they hold the spec citations for each slide.

## Publishing

`.github/workflows/pages.yml` deploys the repository as-is on every push to
`master`. One-time setup: in the repository's **Settings → Pages**, set
**Source** to **GitHub Actions**.
