# Cherry2Cherry 🍒

**A private line between *two* people.**

Cherry2Cherry connects two devices directly over an encrypted peer-to-peer line — no chat server ever sees your messages, because there isn't one.

No accounts. No servers. Just the two of you.

[Request the trial](https://cherry2cherry.space/index.html#request) · [How it works](#how-it-works) · [Trust & verification](#dont-take-our-word-for-it)

---

## Built to have as few places to trust as possible

Every feature exists to keep your conversation between the two of you — not to collect it, back it up, or route it through anyone else.

- **End-to-end encrypted** — Every message and image is encrypted on your device before it ever leaves it, using fresh keys generated new each session.
- **Works fully offline** — No internet at all, if you don't want it — exchange a short code by hand or QR to link two devices on the same network.
- **No accounts, ever** — Nothing to sign up for. Your identifier is a random string generated fresh each time you open the app — never tied to who you are.
- **Send photos too** — Images are compressed and encrypted the same way as text, right in your browser, before they're sent.
- **Three ways to look at it** — Dark, Light, or Cherry — pick the theme that fits your eyes and your mood, not just the operating system default.
- **Runs from one file** — Cherry2Cherry is a single HTML file. Nothing to install, nothing hosted by us — you can even run it straight off your own device.

## How it works

Every connection follows the same short path, whether you're online or completely offline.

1. **Share your ID** — Send your short connection ID — by text, QR code, or a hand-typed offline invite — to the person you want to talk to.
2. **Compare the safety number** — Once linked, both screens show a matching code. Read it out on a call or in person to confirm no one's in the middle.
3. **Talk, encrypted** — From here every message and photo travels straight between your two devices, encrypted the whole way.

## Don't take our word for it

Cherry2Cherry is built so you can check its claims yourself, not just read them.

- ✅ One plain HTML file — open it in any text editor and read exactly what it does.
- ✅ A live network-activity counter shows every request the app makes, in real time.
- ✅ Messages are only ever saved locally, on your own device, if you choose to save them.
- ✅ Offline mode makes zero network requests of its own — verifiably, not just by claim.
- ✅ Not reachable by the EU's current "Chat Control" scanning rule — there's no provider or server here to opt into scanning in the first place.

> **Why this matters:** most chat apps ask you to trust a company, a server, and a privacy policy. Cherry2Cherry tries to need as little trust as possible — the code is short enough to actually read, and open enough to actually verify.
>
> **On "Chat Control":** the EU's current rule (reinstated July 2026, running to 2028) only lets platforms *voluntarily* scan unencrypted messages — it was never able to reach end-to-end encrypted traffic like this app's, and there's no central service here to opt in either way. A separate, permanent proposal ("Chat Control 2.0") that could someday require scanning before encryption is still being negotiated and isn't law — worth knowing about, even if it doesn't change anything here today.

## Verify your download

Only ever get Cherry2Cherry from [cherry2cherry.space](https://cherry2cherry.space) or this repo. If you received a copy some other way, check its checksum against the ones below before you trust it — if even one character doesn't match, the file has been altered and you shouldn't run it. These are published here, separately from the file itself, precisely so a tampered copy can't also fake its own "official" checksum.

| File | Version | SHA-256 |
|---|---|---|
| `cherry2cherry.html` | v0.1.7 | `6a25372d8ee1f6da59d539dfeb90d7b7fc7542639e543722ebb80fa1aebdff71` |
| `IPhone.html` | v0.1.7 | `00cf54ec11ea7380b19bb4cc537d8aba31da162a011868d3bab5035445dad78f` |
| `cherry2cherry-cd.html` | v0.1.7 | `b0f2bca59096145438ca44930e4e1ba768f514878caa8934f3f7b1ba7227c586` |

<details>
<summary>Previous versions</summary>

| File | Version | SHA-256 |
|---|---|---|
| `cherry2cherry.html` | v0.1.6 | `a377a4cbaefdde07aa63a585e3ce0c3d9e39b02ce4383c3580076f119b91c068` |
| `IPhone.html` | v0.1.6 | `3a30a900c65f531fa54c6bd79387e22be27b0a3eec05b3f276120c6c6785b8c8` |

If you have a genuine copy from before an update — a CD burned earlier, for instance — it's still officially valid. It'll match an older checksum here, not the current one, and that's expected: the app's own checker recognizes older official releases too, not just the latest.

</details>

**Check it yourself:**

```bash
# Mac / Linux
shasum -a 256 cherry2cherry.html

# Windows (PowerShell)
certutil -hashfile cherry2cherry.html SHA256
```

These checksums are for v0.1.7 specifically — any future update to the file will have a different one. Whoever publishes a new version should update this list, `checksums.json`, and this README at the same time.

The app itself can also check this for you automatically — the **"Verify this copy"** button on its Me tab compares its own checksum against [`checksums.json`](checksums.json), hosted alongside this page.

## Also available on physical media

Because Cherry2Cherry is just one self-contained HTML file, it works exactly the same burned onto a CD as it does downloaded or hosted. That's a genuine extra layer of security, not just a novelty: a finalized CD is physically read-only — once it's burned, nothing on the network, and no one with remote access to a server, can silently alter the copy sitting on that disc. The only way to change what's on it is to physically have it and burn a new one. Combined with the checksum above, a CD copy is about as tamper-evident as a copy of this app can get.

There's a dedicated build for this, `cherry2cherry-cd.html` — identical to the regular version, except "Clear history on close" starts switched on by default, so nothing lingers in a computer's browser after you eject the disc. (A browser can't actually detect that a file came from a CD specifically — this build just assumes it, rather than relying on you to remember to flip the switch yourself.)

## Files in this repo

| File | What it's for |
|---|---|
| `index.html` | This project's landing page. |
| `cherry2cherry.html` | The standard build — download it and open it directly, no hosting needed. |
| `IPhone.html` | The hosted build — use this URL directly if you're on iPhone, since Safari requires a secure, hosted address to run this app at all. |
| `cherry2cherry-cd.html` | Same app, meant for burning to a CD or other removable media — "Clear history on close" defaults on. |
| `checksums.json` | Machine-readable checksums, used by the app's own "Verify this copy" feature and by anyone checking a copy by hand. |

## Getting it

- **iPhone:** open [cherry2cherry.space/IPhone.html](https://cherry2cherry.space/IPhone.html) directly — this is required due to a Safari limitation with local files.
- **Desktop / Android:** download `cherry2cherry.html` and open it directly in your browser. No install, no server.
- **Removable media:** download `cherry2cherry-cd.html` and burn it to a CD or USB drive.

## Requesting a trial

Want a copy, or to weigh in on which version(s) you'd like (link, file, or CD)? [Request it here](https://cherry2cherry.space/index.html#request), or email **aftercup@aftercup.space** directly.

---

*Unaudited, hand-built encryption — treat it as a solid, transparent prototype, not a substitute for audited tools when the stakes are extremely high. See the in-app info panel for full details on what this does and doesn't protect against.*
