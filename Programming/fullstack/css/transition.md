> **⭐ Interview Question**
> 
> **Difference between Transition and Animation?**
> 
> - **Transition** → Starts when a property changes (e.g., hover, focus).
> - **Animation** → Can run automatically using `@keyframes`, without user interaction.

---

# 28. Transition ⭐⭐⭐

## What is Transition?

The `transition` property creates a **smooth change** between CSS property values.

Without Transition

```
Hover↓Instant Change
```

With Transition

```
Hover↓Smooth Animation
```

Used for

- Buttons
- Cards
- Images
- Links
- Forms
- Menus

---

# Transition Syntax

```
transition: property duration timing-function delay;
```

Example

```
transition: background-color 0.3s ease;
```

---

# Transition Properties ⭐⭐⭐⭐⭐

A transition has **4 parts**.

```
Property

↓

Duration

↓

Timing Function

↓

Delay
```

---

# 1. transition-property ⭐⭐⭐

Specifies which CSS property will animate.

Example

```
transition-property:background-color;
```

Multiple Properties

```
transition-property:background-color,transform;
```

Most Common

```
transition-property:all;
```

Animates all supported property changes.

---

# 2. transition-duration ⭐⭐⭐⭐⭐

Defines how long the transition lasts.

Example

```
transition-duration:0.3s;
```

Other Examples

```
transition-duration:500ms;transition-duration:1s;
```

Most websites use

```
0.2s0.3s0.5s
```

---

# 3. transition-timing-function ⭐⭐⭐⭐

Controls the animation speed.

Common Values

```
easelinearease-inease-outease-in-out
```

### ease (Default)

Starts slow, speeds up, then slows down.

```
transition-timing-function:ease;
```

---

### linear

Same speed throughout.

```
transition-timing-function:linear;
```

---

### ease-in

Starts slowly.

```
transition-timing-function:ease-in;
```

---

### ease-out

Ends slowly.

```
transition-timing-function:ease-out;
```

---

### ease-in-out

Smooth start and end.

```
transition-timing-function:ease-in-out;
```

---

# 4. transition-delay ⭐⭐

Waits before starting.

Example

```
transition-delay:0.5s;
```

The animation begins after **0.5 seconds**.

---

# Transition Shorthand ⭐⭐⭐⭐⭐

Instead of

```
transition-property:transform;transition-duration:0.3s;transition-timing-function:ease;
```

Use

```
transition:transform 0.3s ease;
```

Most commonly used.

---

# Complete Example ⭐⭐⭐⭐⭐

```
button{transition:background-color 0.3s ease;}button:hover{background-color:blue;}
```

---

# Multiple Transitions ⭐⭐⭐⭐

```
transition:background-color 0.3s ease,transform 0.3s ease;
```

---

# Common Hover Effects

### Button

```
button{transition:0.3s;}button:hover{background:blue;}
```

---

### Card Lift

```
.card{transition:transform 0.3s ease;}.card:hover{transform:translateY(-8px);}
```

---

### Image Zoom

```
img{transition:transform 0.3s ease;}img:hover{transform:scale(1.1);}
```

---

### Link Color

```
a{transition:color 0.3s ease;}a:hover{color:red;}
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|transition|⭐⭐⭐⭐⭐|
|transition-duration|⭐⭐⭐⭐⭐|
|transition-timing-function|⭐⭐⭐⭐|
|transition-property|⭐⭐⭐|
|transition-delay|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Shorthand

```
transition:0.3s;
```

---

### Transform

```
transition:transform 0.3s ease;
```

---

### Background

```
transition:background-color 0.3s ease;
```

---

### Delay

```
transition-delay:0.5s;
```

---

### Multiple

```
transition:transform 0.3s,opacity 0.3s;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. transition:0.3s ⭐⭐⭐⭐⭐2. transition:transform 0.3s ease ⭐⭐⭐⭐⭐3. transition:background-color 0.3s ease ⭐⭐⭐⭐4. transition:opacity 0.3s ⭐⭐⭐⭐5. transition-delay ⭐⭐
```

---

# 💡 Full Stack Tip

These are the transition patterns you'll use almost every day:

### Card Hover

```
.card{    transition:transform 0.3s ease;}.card:hover{    transform:translateY(-8px);}
```

---

### Button Hover

```
button{    transition:background-color 0.3s ease;}button:hover{    background-color:#2563eb;}
```

---

### Image Hover

```
img{    transition:transform 0.3s ease;}img:hover{    transform:scale(1.05);}
```

> **Best Practice:** Avoid `transition: all;` unless you truly want every animatable property to transition. It's generally better for performance and predictability to specify only the properties you want to animate, such as `transform`, `opacity`, or `background-color`.