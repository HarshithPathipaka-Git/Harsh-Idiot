> **⭐ Interview Question**
> 
> **Transition vs Animation**
> 
> - **Transition** → Runs when a property changes (hover, focus, click, etc.).
> - **Animation** → Can run automatically or repeatedly using `@keyframes`.

---

# 29. Animation ⭐⭐⭐⭐

## What is Animation?

CSS Animations allow elements to **change their appearance over time**.

They can

- Move
- Rotate
- Fade
- Scale
- Change Colors
- Repeat Automatically

Used for

- Loading Spinners
- Hero Sections
- Icons
- Buttons
- Cards
- Notifications

---

# How Animation Works ⭐⭐⭐⭐⭐

CSS Animations require **2 steps**.

### Step 1

Create animation using

```
@keyframes
```

### Step 2

Apply it using

```
animation
```

---

# 1. @keyframes ⭐⭐⭐⭐⭐

Defines the animation.

Syntax

```
@keyframes animation-name{}
```

Example

```
@keyframes move{from{    transform:translateX(0);}to{    transform:translateX(200px);}}
```

---

## Using Percentages

Instead of `from` and `to`

```
@keyframes fade{0%{opacity:0;}50%{opacity:0.5;}100%{opacity:1;}}
```

Most professional animations use percentages.

---

# 2. Animation Properties ⭐⭐⭐⭐⭐

Animations are controlled using several properties.

---

## animation-name ⭐⭐⭐⭐

Specifies which animation to run.

```
animation-name:move;
```

---

## animation-duration ⭐⭐⭐⭐⭐

How long the animation runs.

```
animation-duration:2s;
```

---

## animation-timing-function ⭐⭐⭐⭐

Controls animation speed.

Values

```
easelinearease-inease-outease-in-out
```

Example

```
animation-timing-function:ease;
```

---

## animation-delay ⭐⭐⭐

Wait before starting.

```
animation-delay:1s;
```

---

## animation-iteration-count ⭐⭐⭐⭐

How many times the animation repeats.

Once

```
animation-iteration-count:1;
```

Infinite

```
animation-iteration-count:infinite;
```

---

## animation-direction ⭐⭐⭐

Controls the animation direction.

Values

```
normalreversealternatealternate-reverse
```

Example

```
animation-direction:alternate;
```

---

## animation-fill-mode ⭐⭐⭐

Controls the element's appearance before and after the animation.

Values

```
noneforwardsbackwardsboth
```

Example

```
animation-fill-mode:forwards;
```

Keeps the final animation state after it finishes.

---

## animation-play-state ⭐⭐

Controls whether the animation is running.

Values

```
runningpaused
```

Example

```
animation-play-state:paused;
```

---

# Animation Shorthand ⭐⭐⭐⭐⭐

Instead of

```
animation-name:move;animation-duration:2s;animation-timing-function:ease;animation-iteration-count:infinite;
```

Use

```
animation:move 2s ease infinite;
```

Syntax

```
animation:namedurationtiming-functiondelayiteration-countdirectionfill-modeplay-state;
```

---

# Complete Example ⭐⭐⭐⭐⭐

```
@keyframes bounce{0%{    transform:translateY(0);}50%{    transform:translateY(-20px);}100%{    transform:translateY(0);}}.ball{animation:bounce 1s ease infinite;}
```

---

# Common Animations

### Fade In

```
@keyframes fade{from{    opacity:0;}to{    opacity:1;}}
```

---

### Rotate

```
@keyframes spin{from{    transform:rotate(0deg);}to{    transform:rotate(360deg);}}
```

---

### Scale

```
@keyframes zoom{from{    transform:scale(1);}to{    transform:scale(1.2);}}
```

---

### Slide

```
@keyframes slide{from{    transform:translateX(-100px);}to{    transform:translateX(0);}}
```

---

# Transition vs Animation ⭐⭐⭐⭐⭐

|Transition|Animation|
|---|---|
|Triggered by a change|Can run automatically|
|Usually one state change|Multiple keyframes|
|Simpler|More powerful|
|Hover effects|Loading, banners, logos|

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|@keyframes|⭐⭐⭐⭐⭐|
|animation|⭐⭐⭐⭐⭐|
|animation-duration|⭐⭐⭐⭐⭐|
|animation-iteration-count|⭐⭐⭐⭐|
|animation-timing-function|⭐⭐⭐⭐|
|animation-name|⭐⭐⭐|
|animation-direction|⭐⭐⭐|
|animation-fill-mode|⭐⭐⭐|
|animation-delay|⭐⭐|
|animation-play-state|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Keyframes

```
@keyframes move{from{}to{}}
```

---

### Apply Animation

```
animation:move 2s ease;
```

---

### Infinite

```
animation-iteration-count:infinite;
```

---

### Alternate

```
animation-direction:alternate;
```

---

### Keep Final State

```
animation-fill-mode:forwards;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. @keyframes ⭐⭐⭐⭐⭐2. animation ⭐⭐⭐⭐⭐3. animation-duration ⭐⭐⭐⭐⭐4. animation-iteration-count ⭐⭐⭐⭐5. animation-timing-function ⭐⭐⭐⭐6. animation-direction ⭐⭐⭐7. animation-fill-mode ⭐⭐⭐8. animation-delay ⭐⭐9. animation-play-state ⭐⭐
```

---

# 💡 Full Stack Tip

These are the animation patterns you'll encounter most often:

### Loading Spinner

```
@keyframes spin{from{    transform:rotate(0deg);}to{    transform:rotate(360deg);}}.spinner{    animation:spin 1s linear infinite;}
```

---

### Fade In

```
.fade{    animation:fade 0.5s ease;}
```

---

### Bounce

```
.ball{    animation:bounce 1s ease infinite;}
```

> **Best Practice:** Prefer **`transform`** and **`opacity`** inside animations because they are generally more performant than animating layout-affecting properties like `width`, `height`, `top`, or `left`.

---

## 🚀 Animation Cheat Sheet (Remember These 5)

```
@keyframesanimationanimation-durationanimation-iteration-countanimation-timing-function
```

These five cover the majority of CSS animations you'll write.