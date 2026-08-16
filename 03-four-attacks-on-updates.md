# What Can Go Wrong?

Eve isn't limited to one trick. Here are four different ways she can attack an update system.

### Attack 1: The Fake Update

```
Alice → publishes Update v2
Eve   → sends Bob a malware file disguised as v2
```

> **Question:** How can Bob know the update he received was really *made* by Alice?

### Attack 2: The Old Version Attack

```
Real latest version = v5
Eve gives Bob        = v2 (old, with known bugs/vulnerabilities)
```

> **Question:** How can Bob know he's not being fed an outdated, less-secure version — even if it's a *genuine* file Alice once published?

### Attack 3: The Missing Update Attack

```
Real latest version = v5
Eve keeps serving Bob v4, forever
```

> **Question:** How can Bob even know a newer version exists, if Eve controls what he sees?

### Attack 4: The Compromised Key

```
Eve steals one of Alice's signing keys
```

> **Question:** If Eve now has a "real" key, is the whole system broken?

These four questions are the heart of the problem. Everything TUF does is designed to answer them.

---

*This page can later be adapted into a standalone contribution connecting attacks to TUF mechanisms.*
