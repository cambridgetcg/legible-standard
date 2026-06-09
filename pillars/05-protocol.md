# 05. Protocol — how systems talk, so anyone can listen

**We hold:**

- A protocol (the agreed way systems talk) belongs to everyone who uses it, not to whoever wrote it first.
- Open formats (ones anyone can read and use for free) come first; a closed one needs a written reason.
- A machine and a person can both read every message we send — the same message.
- The old way keeps working. Before it stops, we say so — loudly and early.
- An interface (a door into a system) is not finished until we write down how it works.

**Do:**

- Publish every interface twice: in plain words for people, and in a spec (an exact, formal description) for machines.
- Use open formats before we invent our own.
- Give every change a version number: name it, date it, write what changed and why.
- Keep the old version working when we release a new one, and say exactly how long it will live.
- Announce breaking changes (changes that stop old things from working) before they happen, never after.
- Give every interface one complete example that a stranger can copy, paste, and run.
- For every machine message, offer a view a person can read — one command or one click away.
- Pick the open standard that already exists instead of building a private one.

**Don't:**

- Don't break the old way silently. Ever.
- Don't pick a proprietary (one-owner) format or tool when an open one does the job.
- Don't hide what a system does behind doors (endpoints), switches (flags), or side paths that no document mentions.
- Don't send a message that only a machine can read, or only a person can read.
- Don't change what a message means without changing its version number.

**Why:**

Machines talk to each other far more than people do, and most of that talk is about you — your money, your messages, your records. When systems speak a secret language, only their owner can check what they say. Everyone else just has to trust. When systems speak openly, anyone can build a new piece, fix a broken one, or replace one that turned bad — today or in ten years. And when we change how we speak, we say so first, so nothing you built on our word dies quietly in the night.

**The test:**

Could a stranger build something that talks to our system, using only our public documents — and would it still work after our next update?
