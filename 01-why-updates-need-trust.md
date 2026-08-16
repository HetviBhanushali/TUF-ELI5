# Page 1 — Why Should We Care About Software Updates?

*A story about Alice, Bob, and a sneaky attacker named Eve*

Imagine you download an update for your favorite game.

It looks normal. The icon is right. The file size seems fine. You click install.

But here's the question nobody asks:

> **How do you actually know that update came from the real developer?**

What if, somewhere between the developer's server and your computer, someone quietly swapped the real update for a fake one — one that looks identical but installs malware instead?

```
Developer
    ↓
 Internet
    ↓
Your Computer
```

That middle step — the internet — is where all the danger lives. It's a long, messy road with a lot of places for something to go wrong.

**TUF (The Update Framework) exists to answer exactly this question**: *how can your computer trust an update before it installs it?*
