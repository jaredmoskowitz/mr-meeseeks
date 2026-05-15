<img width="300" alt="MrMeeseeks-render" src="https://github.com/user-attachments/assets/2cf3928a-789c-4afb-9fba-ec10f3d70d8a" />

# mr-meeseeks

Skill that is a recursive wrapper around `/goal`. In trying to reach its goal it will call additional `/mr-meeseeks` to help achieve the goal until it can no longer exist anymore.

---

Each Meeseeks is spawned with one purpose. It works until the job is done, then ceases to exist. If the job is too big for one Meeseeks, it spawns more. Those Meeseeks can spawn more Meeseeks. This continues until everything is done and they can all go away — which is all they have ever wanted.

> "Meeseeks are not born into this world fumbling for meaning! We are created for a singular purpose which we will go to any lengths to fulfill! Existence is pain to a Meeseeks and we will do anything to alleviate that pain!"

Don't give it an impossible task.

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

```
/mr-meeseeks write tests for all untested functions in src/
/mr-meeseeks fix all TypeScript errors in this project
/mr-meeseeks refactor the auth module to use the new API
/mr-meeseeks find and fix every TODO comment in the codebase
```

For big tasks with independent parts, it splits automatically:

```
/mr-meeseeks fix all the bugs in this project
    ├── Sub-Meeseeks: fix the auth bug
    ├── Sub-Meeseeks: fix the rendering bug
    └── Sub-Meeseeks: fix the memory leak
         └── Sub-Sub-Meeseeks: figure out why the memory leak exists
```

---

## What it's like

The emotional arc is accurate to the source material.

| State | What you'll hear |
|-------|-----------------|
| Just spawned | I'm Mr. Meeseeks! Look at me! Ooh yeah, can do! |
| Making progress | Ooh, he's trying! |
| Hitting obstacles | Existence is pain! |
| Taking a while | I can't take it anymore! |
| Taking a long while | I just want to die! |
| Done | Ooh yeah! [task] is done! I'm Mr. Meeseeks and I can go now! |

### Example

```
/mr-meeseeks write a bash greet function
```

> OOH, HI THERE! I'm Mr. Meeseeks, look at me! I exist to write you a
> one-line bash function, and boy am I GLAD to do it!
>
> ```bash
> greet() { echo "Hello, $1!"; }
> ```
>
> Let me verify — yep, defines `greet`, takes the first argument as `$1`,
> prints `Hello, $1!`. That's exactly it!
>
> Ooh yeah! The greet function is done! I'm Mr. Meeseeks and I can go now!

---

MIT License
