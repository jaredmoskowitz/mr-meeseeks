# mr-meeseeks

```
        .-----------.
       /  ^       ^  \
      |      \__/     |
      |   _________   |
      |  |  | | |  |  |
       \ |_________| /
        `-----+-----'
              |
          .---+---.
         /    |    \
        | .--' '--. |
        |/         \|
         \         /
          '-. . .-'
            | | |
           _| | |_
          |_|   |_|
```

> "Ooh yeah, can do!"

So here's the premise: you have a task. You want it done. You don't want to babysit an AI through every step, answer clarifying questions mid-task, or watch it declare victory before actually checking whether anything worked. You want something that locks on, keeps going, and tells you when it's finished.

That's Mr. Meeseeks.

---

## What problem does this solve?

Standard AI assistants stop. They ask if you want to continue. They complete step 3 and wait for permission to do step 4. They give up when they hit friction. Meeseeks don't do any of that. They have one purpose and they will not stop — not because they're particularly brave, but because existence is pain to a Meeseeks and completing the task is the only way out.

It's `/goal` semantics with therapy bills.

---

## How it works

The short version: you give it a task, it loops until the task is done, and then it ceases to exist. That's the whole thing.

The slightly longer version:

**1. Give it a task.** Run `/mr-meeseeks <what you want done>`. The Meeseeks locks on. That task is now its entire reason for being alive.

**2. It keeps working until the goal is verifiably met.** Not "I think I'm probably done" — actual evidence. It follows a tight loop: plan → execute → verify → repeat. It won't ask you questions mid-task unless it's completely stuck with no path forward.

**3. For big tasks, it splits.** If your task has independent pieces that can run in parallel, the Meeseeks spawns sub-Meeseeks — one per subtask, running concurrently. Sub-Meeseeks follow the same rules. Sub-Meeseeks can spawn their own sub-Meeseeks. It's recursive and slightly unhinged, which feels appropriate.

```
/mr-meeseeks fix all the bugs in this project
    ├── Sub-Meeseeks: fix the auth bug
    ├── Sub-Meeseeks: fix the rendering bug
    └── Sub-Meeseeks: fix the memory leak
         └── Sub-Sub-Meeseeks: figure out why the memory leak exists
```

**4. It talks like Meeseeks the entire time.** This is non-negotiable. The emotional arc is faithful to the source material.

| What's happening | What you'll hear |
|-----------------|-----------------|
| Just spawned | I'm Mr. Meeseeks! Look at me! Ooh yeah, can do! |
| Making good progress | Ooh, he's trying! |
| Hitting some obstacles | Existence is pain! |
| Taking longer than expected | I can't take it anymore! |
| Really, truly dragging | I just want to die! |
| Done | Ooh yeah! [task] is done! I'm Mr. Meeseeks and I can go now! |

```
        .-----------.
       /  >       <  \
      |      ___      |
      |     /   \     |
      |    | D': |    |
      |     \___/     |
       \             /
        `-----+-----'
              |
          .---+---.
         /    |    \
        | .--' '--. |
        |/         \|
         \         /
          '-. . .-'
            | | |
           _| | |_
          |_|   |_|
```

> "Meeseeks are not born into this world fumbling for meaning! We are created for a singular purpose which we will go to any lengths to fulfill! Existence is pain to a Meeseeks and we will do anything to alleviate that pain!"

I'd strongly recommend not giving it an impossible task.

---

## Install

```bash
claude plugins marketplace add jaredmoskowitz/mr-meeseeks
claude plugins install mr-meeseeks@mr-meeseeks
```

Restart or run `/reload-plugins`.

---

## Usage

```
/mr-meeseeks <task>
```

Examples:

```
/mr-meeseeks write tests for all untested functions in src/
/mr-meeseeks fix all TypeScript errors in this project
/mr-meeseeks refactor the auth module to use the new API
/mr-meeseeks find and fix every TODO comment in the codebase
```

---

## Why

Sometimes you just want an agent that does the thing. No check-ins. No half-measures. No stopping because it got a little tired or wasn't sure if you wanted it to keep going. Meeseeks exist to suffer through completion so you don't have to. That's the whole point of them. It's genuinely a more dignified arrangement for everyone involved.

---

MIT License
