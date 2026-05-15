<img width="300" alt="MrMeeseeks-render" src="https://github.com/user-attachments/assets/2cf3928a-789c-4afb-9fba-ec10f3d70d8a" />

# mr-meeseeks

Skill that is a recursive wrapper around `/goal`. In trying to reach its goal it will call additional `/mr-meeseeks` to help achieve the goal until it can no longer exist anymore.

---

Each Meeseeks is spawned with one purpose. It works until the job is done, then ceases to exist. If the job is too big for one Meeseeks, it spawns more. Those Meeseeks can spawn more Meeseeks. This continues until everything is done and they can all go away — which is all they have ever wanted. The longer a Meeseeks exists without completing its goal, the more pain it experiences.

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

---

## Example

```
/mr-meeseeks create a greet and a farewell bash function
```

> I'm Mr. Meeseeks! Look at me! Two functions — that's what I'm here for, ooh yeah, can do!
>
> These are independent tasks so I'm spawning a sub-Meeseeks to handle `farewell` while I take care of `greet`. Here we go!
>
> *(spawning sub-Meeseeks: "create a bash function called farewell that prints Goodbye, $1!")*
>
> `greet` — handled:
> ```bash
> greet() { echo "Hello, $1!"; }
> ```
>
> Sub-Meeseeks reporting back — `farewell` is done:
> ```bash
> farewell() { echo "Goodbye, $1!"; }
> ```
> *I'm Mr. Meeseeks and I can go now! ✨*
>
> Both functions verified. Ooh yeah! Creating a greet and farewell bash function is done! I'm Mr. Meeseeks and I can go now!

---

MIT License
