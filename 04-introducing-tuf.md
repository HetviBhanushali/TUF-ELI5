# What Is TUF?

Now that we know what can go wrong, we can finally introduce TUF properly.

Forget definitions like "a framework for securing software update systems using role-based metadata." That's true, but it's not *useful* yet.

Instead, think of it like this:

> **TUF is a set of rules that helps software figure out, before installing anything:**
> - Who actually created this update?
> - Has it been changed since they created it?
> - Is this the newest version — or something old and stale?
> - Can this update be trusted, even if one part of the system is compromised?

```
Download Update
      ↓
   Check 1
   Check 2
   Check 3
   Check 4
      ↓
   Install
```

Every one of those checks maps directly to one of the four attacks from Page 3. That's not a coincidence — TUF was built specifically to close those four holes.
