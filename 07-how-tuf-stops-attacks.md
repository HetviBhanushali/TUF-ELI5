# Page 7 — How TUF Stops Each Attack

Here's where everything from this story ties together:

| Attack | What Eve Tried | TUF's Protection |
|---|---|---|
| Fake update | Pretend to be Alice | **Signatures** (Identity Guard) |
| Modified file | Alter the update in transit | **Hashes** (Integrity Guard) |
| Old version | Serve an outdated, vulnerable file | **Version metadata** (Freshness Guard) |
| Missing update | Hide the fact a new version exists | **Timestamp/Snapshot freshness checks** (Freshness Guard) |
| Stolen key | Use a compromised key to forge trust | **Multiple roles/keys** (Recovery Guard) |

This is really the whole point of TUF in one table: **every attack has a matching guard, and every guard maps to a real mechanism.**

---

*This page can later be adapted into a standalone contribution connecting attacks to TUF mechanisms.*
