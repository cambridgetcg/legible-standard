# 04. Security — guard for real, not for show

**We hold:**

1. We protect what matters. We skip things that only look safe but stop nothing.
2. A secret (password, key, token) never appears in code, logs, or chat — only the name of the file that holds it.
3. Once a secret leaks, it is dead. Deleting your copy does not delete the copies others made — so we rotate it (replace it with a new one).
4. Every person and every tool gets only the access it needs for its job — no more.
5. When something goes wrong, we say it early and in plain words. Hiding it does more harm than the break-in itself.

**Do:**

1. Keep every secret in a file that git ignores (like `.env`). Commit (save into git) only a blank example of it.
2. Rotate a secret the moment it touches a commit, a log, or a screen share — no exceptions, no debate.
3. Turn on 2FA (two-step login) for every account that offers it, starting with email and code hosting (like GitHub).
4. Give each person, tool, and key only the access its one job needs. Remove that access the day the job ends.
5. Before every release, scan your code and your dependencies (borrowed code) for known holes.
6. Every three months, review who has access to what. Remove any access that nobody can explain.
7. When an incident (security failure) happens, publish three things fast: what happened, when, and what we are doing now.
8. Write down how people can report a security problem to us — and thank anyone who does.

**Don't:**

1. Don't commit a secret, ever. Removing it from git later does not fix the leak — the secret is already out, so rotate it.
2. Don't print, paste, or log a secret's value — name the file, never the contents.
3. Don't let people share one account or one key. If everyone shares a key, nobody can say who did what.
4. Don't add security steps that slow people down but stop no attacker — that is just for show.
5. Don't hide an incident, make it sound smaller, or wait for perfect wording. Speak first, polish later.
6. Don't grant "admin for now, we'll tighten later" — later never comes.

**Why:**

Locks only help if they are on the right doors. A password pasted into code is like a key left
in the lock. Taking the key back does not destroy the copies others may already have made.
That is why we change the lock instead of pretending. Giving everyone the smallest access that
works means one mistake stays one mistake. And when we do fail, we say so fast and in plain
words — that lets people protect themselves, which is the whole point of guarding anything.

**The test:** Can we show, today, where every secret lives, who can touch each one, and the plain note we published the last time one leaked?
