<div align="center">

# Gaurav Bhandari

Software engineer at PagarBook. After hours I write small, fast native apps for my Mac and raise a language model from scratch.

<a href="https://www.linkedin.com/in/gaurav-bhandari-171o/"><img src="https://img.shields.io/badge/LinkedIn-Gaurav%20Bhandari-0A66C2" alt="LinkedIn"></a>
<a href="https://x.com/kratosRespawned"><img src="https://img.shields.io/badge/X-@kratosRespawned-000000?logo=x&logoColor=white" alt="X"></a>
<a href="mailto:sbhandari1907@protonmail.com"><img src="https://img.shields.io/badge/Email-sbhandari1907@protonmail.com-6D4AFF?logo=protonmail&logoColor=white" alt="Email"></a>

</div>

## Stuff I'm currently building

<table>
<tr>
<td width="33%" valign="top">
<p align="center">
<img src="assets/masks.png" width="80" alt="Masks icon"><br>
<b>Masks</b><br>
An agent-first browser where every tab wears a mask<br><br>
<img src="https://img.shields.io/badge/binary-2.9%20MB-blue" alt="2.9 MB binary">
<img src="https://img.shields.io/badge/dependencies-0-brightgreen" alt="0 dependencies">
<img src="https://img.shields.io/badge/repo-private-lightgrey" alt="Private repo">
</p>
<ul>
<li>Every tab has its own login identity</li>
<li>AI agents drive it over a CLI and MCP, and see only the tabs I share</li>
<li>Saved flows run headless on a cron</li>
<li>Sandboxed, with no telemetry</li>
</ul>
</td>
<td width="33%" valign="top">
<p align="center">
<a href="https://github.com/kratos-respawned/hop"><img src="assets/hop.png" width="80" alt="Hop icon"></a><br>
<b><a href="https://github.com/kratos-respawned/hop">Hop</a></b><br>
A macOS launcher with dev tools built in<br><br>
<img src="https://img.shields.io/badge/binary-1.4%20MB-blue" alt="1.4 MB binary">
<img src="https://img.shields.io/badge/dependencies-0-brightgreen" alt="0 dependencies">
<img src="https://img.shields.io/badge/keystroke-under%200.3%20ms-orange" alt="Under 0.3 ms per keystroke">
</p>
<ul>
<li>App search, clipboard history, a calculator and a video downloader</li>
<li>An AirDrop shelf at the notch</li>
<li>Dev tools for ports, worktrees and whatever is heating the Mac</li>
</ul>
</td>
<td width="33%" valign="top">
<p align="center">
<img src="assets/burrow.png" width="80" alt="Burrow icon"><br>
<b>Burrow</b><br>
A Finder replacement for developers<br><br>
<img src="https://img.shields.io/badge/binary-0.9%20MB-blue" alt="0.9 MB binary">
<img src="https://img.shields.io/badge/dependencies-0-brightgreen" alt="0 dependencies">
<img src="https://img.shields.io/badge/repo-private-lightgrey" alt="Private repo">
</p>
<ul>
<li>Folders list through native kernel calls</li>
<li>Search on its own index that skips <code>node_modules</code> and build folders</li>
<li>Git branch and sibling worktrees in the status bar</li>
</ul>
</td>
</tr>
</table>

All three are plain Swift and AppKit.

### Security work inside Masks

<table>
<tr>
<td width="130"><b>Passkeys</b></td>
<td>An authenticator written from scratch. I implemented WebAuthn by hand, keys stay in the Secure Enclave behind Touch ID, and a passkey on a phone signs in by QR code and Bluetooth over the CTAP hybrid transport.</td>
</tr>
<tr>
<td><b>Notifications</b></td>
<td>End-to-end encrypted. My Web Push relay on Cloudflare Workers carries messages it cannot read or forge, and every device signs its requests with a P-256 key.</td>
</tr>
<tr>
<td><b>Private line</b></td>
<td>Masks can hand a download to Hop along with the site login it needs. Each app verifies the other's code signature before any request moves, so no other process can pose as either app.</td>
</tr>
</table>

## Vani

A language model I am raising from scratch on my laptop.

<table>
<tr>
<td width="25%" align="center" valign="top"><h3>2 to 8</h3>layers, grown as she read more</td>
<td width="25%" align="center" valign="top"><h3>7.5M</h3>parameters</td>
<td width="25%" align="center" valign="top"><h3>4 to ~182</h3>right out of 226 on an exam she was never taught</td>
<td width="25%" align="center" valign="top"><h3>870</h3>lines of PyTorch in one file</td>
</tr>
</table>

- Every day ends in sleep, when she replays her memories in dreams and learns from them.
- Seven hormone-like scores, dopamine, cortisol and curiosity among them, decide when she is tired, scared, or curious enough to pick her own book.

## At PagarBook

I work across the backend, the web app, the mobile apps and the desktop.

- **Face recognition engine**, built in-house from scratch.
- **Device management** for the attendance kiosks.
- **SignX**, a Tauri desktop app that signs Form 16 PDFs in bulk with a Class 3 DSC USB token and ships as a 2.7 MB installer. Everything below the UI is low-level Rust with a hand-written PDF writer. A few wrong PINs lock a token for good, so every check that needs no PIN runs first, and one PIN entry signs the whole batch.

## Tools

<img src="https://skillicons.dev/icons?i=swift,rust,ts,react,nextjs,nodejs,postgres,cloudflare,pytorch,tauri" alt="Swift, Rust, TypeScript, React, Next.js, Node.js, Postgres, Cloudflare, PyTorch, Tauri">
