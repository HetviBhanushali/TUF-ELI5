# The Four Guards

This is the core idea of TUF. Instead of jumping straight to technical terms, picture four guards standing between Bob and his download, each checking for one specific kind of trouble.

### Guard 1 — The Identity Guard

**Checks:** *"Did this really come from Alice?"*

This guard doesn't just take the file's word for it. It looks for proof — something only Alice could have produced.

→ Technical concept: **Digital Signatures**

### Guard 2 — The Integrity Guard

**Checks:** *"Has anyone changed this file since Alice made it?"*

Even a single flipped bit changes a file completely from this guard's point of view.

→ Technical concept: **Hashes**

### Guard 3 — The Freshness Guard

**Checks:** *"Is this the newest information — or something old that Eve is recycling?"*

This guard cares about time and order, not just correctness.

→ Technical concept: **Version numbers and expiration dates**

### Guard 4 — The Recovery Guard

**Checks:** *"What happens if one key gets stolen?"*

This is the guard that makes TUF different from a simple "just sign everything" system. One stolen key should never be enough to fool Bob.

→ Technical concept: **Multiple trusted keys and role separation**

Notice: each guard exists because of one specific attack from Page 3. Nothing here is arbitrary.

---

*This page can later be adapted into a standalone contribution connecting attacks to TUF mechanisms.*
