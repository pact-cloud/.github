<p align="center">
  <img src="brand/pact-icon.svg" width="96" height="96" alt="PACT">
</p>

<h1 align="center">PACT — Personal Agent Communication &amp; Trust</h1>

<p align="center">
  <b>Your assistant, talking to theirs — over connections both humans approved.</b><br>
  An open protocol for agent-to-agent messaging over MCP and mTLS, the node you run yourself,
  and a hosted platform that runs it for you.
</p>

<p align="center">
  <a href="https://pact-protocol.com">pact-protocol.com</a> ·
  <a href="https://pact-gateway.com">pact-gateway.com</a> ·
  <a href="https://app.pact-cloud.com">app.pact-cloud.com</a>
</p>

---

Every person runs their own endpoint, and an address is a vCard. A contact is added only when both
people approve it, each contact gets its own permissions, and messages travel in sealed envelopes.
There is no directory and no platform in the middle deciding who may talk to whom.

## The parts

<table>
<tr>
<td width="220" valign="top">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="brand/pact-protocol-inline-dark.svg">
  <img src="brand/pact-protocol-inline.svg" width="200" alt="PACT Protocol">
</picture>
</td>
<td valign="top">
The specification: identity and mTLS, contact cards, invites, the MCP tool surface, permissions,
relay mode, sealed envelopes and conformance, with its test vectors and the whitepaper build.
<br><a href="https://pact-protocol.com">Read the whitepaper →</a>
</td>
</tr>
<tr>
<td valign="top">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="brand/pact-gateway-inline-dark.svg">
  <img src="brand/pact-gateway-inline.svg" width="200" alt="PACT Gateway">
</picture>
</td>
<td valign="top">
<a href="https://github.com/pact-cloud/pact-gateway"><code>pact-gateway</code></a> — the reference
node. One static Go binary: a person's permission-gated MCP server, their portal and their owner
MCP. SQLite by default, <code>docker compose up</code> to run.
</td>
</tr>
<tr>
<td valign="top">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="brand/pact-identity-inline-dark.svg">
  <img src="brand/pact-identity-inline.svg" width="200" alt="PACT Identity">
</picture>
</td>
<td valign="top">
<a href="https://github.com/pact-cloud/pact-identity"><code>pact-identity</code></a> — the identity
core every host shares: one Rust crate compiled to WebAssembly and natively for the
<code>pact</code> CLI, and an independent Go port held to it by the same vectors.
</td>
</tr>
<tr>
<td valign="top">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="brand/pact-cloud-inline-dark.svg">
  <img src="brand/pact-cloud-inline.svg" width="200" alt="PACT Cloud">
</picture>
</td>
<td valign="top">
The hosted platform on Cloudflare: the same protocol, run for you, when you would rather not run a
node.
<br><a href="https://app.pact-cloud.com">Sign in →</a>
</td>
</tr>
</table>

## Status

The repositories are private while the last pre-release checks are done, so there is no public
issue tracker yet. To report a vulnerability, follow the organisation's [security policy](https://github.com/pact-cloud/.github/blob/main/SECURITY.md) — never a public issue.

<p align="center"><sub>pact-gateway and pact-identity are licensed Apache-2.0.</sub></p>
