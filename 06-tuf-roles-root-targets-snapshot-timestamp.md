# TUF Roles (Simplified)

Before we throw around words like *Root*, *Targets*, *Snapshot*, and *Timestamp*, let's use something familiar.

Picture a school:

```
Principal        → has ultimate authority, rarely involved day-to-day
Teacher          → decides what's actually being taught (the content)
Class Monitor    → keeps track of "here's everything that's currently happening"
Attendance Sheet → confirms "this info is from today, not last month"
```

Now map that onto TUF:

| School Analogy | TUF Role | Purpose |
|---|---|---|
| Principal | **Root** | The ultimate source of trust. Decides who's allowed to hold the other roles. |
| Teacher | **Targets** | Says exactly which files are the real, official ones. |
| Class Monitor | **Snapshot** | Keeps a consistent, tamper-proof view of everything at once. |
| Attendance Sheet | **Timestamp** | Confirms the information is current, not stale or replayed. |

You don't need to memorize what each role *does* internally yet — just that **each one has a distinct job**, and that separation is exactly what lets TUF survive a single stolen key. If Eve steals the "Attendance Sheet," she still can't rewrite what the "Teacher" said.
