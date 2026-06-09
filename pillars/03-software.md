# 03. Software — code that tells the truth

**We hold:**

1. A README (the front page of the code) is a promise. The code keeps that promise, or the README changes.
2. A claim without a test (a small check that proves the code works) is a rumor.
3. Every dependency (code we borrow) is a debt, and we explain every debt.
4. We write code for the next reader first, the machine second.
5. A feature that hides what it is really doing is lying, even if no one wrote a false word.

**Do:**

- When we change what the code does, update the README in the same change.
- Write the test before we claim the feature works.
- Next to every dependency we add, write one plain sentence saying why we need it.
- Name things so a newcomer can guess what they do before opening them.
- Mark unfinished work where users can see it: "not done yet" beats silence.
- Make errors say what happened and what to do next, in plain words.
- Delete code we no longer maintain instead of letting it rot in place.
- Before each release (each new version we ship), read our own README like a stranger would, and fix what confuses us.

**Don't:**

- Don't ship a button that does nothing.
- Don't describe a planned feature as if it already exists.
- Don't show success when the work failed or is still running.
- Don't add a dependency to save an afternoon and pay for it for a year.
- Don't write clever code where clear code would do the same job.
- Don't print secrets (passwords, keys) anywhere — name the file that holds them, never the secret itself.

**Why:**

Software is the only worker that never sleeps. So when it lies, it lies
thousands of times a day, to people who cannot argue back. A README that no
longer matches the code teaches every new reader something false. A green
checkmark over broken work wastes the time of everyone who trusted it. We keep
our code honest the same way we keep our money honest: we write down every
claim, we check every claim, and anyone — not just an expert — can follow the
trail from the promise to the proof.

**The test:**

If a stranger reads the README, runs the tests, and then reads the code — do all three tell the same story?
