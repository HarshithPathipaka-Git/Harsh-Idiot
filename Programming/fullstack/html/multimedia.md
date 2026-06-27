#  Multimedia

## `<audio>`

**Purpose:** Embeds audio files.

**Syntax**

```html
<audio controls>
```

**Use**

- Music
    
- Podcasts
    
- Voice recordings
    

---

## `<video>`

**Purpose:** Embeds video files.

**Syntax**

```html
<video controls>
```

**Use**

- Tutorials
    
- Movies
    
- Product demos
    

---

## `<source>`

**Purpose:** Specifies alternative media files.

**Example**

```html
<source src="video.mp4" type="video/mp4">
```

**Use**

- Multiple video/audio formats
    
- Responsive media
    

---

## `<track>`

**Purpose:** Adds subtitles, captions, or descriptions to videos.

**Example**

```html
<track src="subtitles.vtt" kind="subtitles">
```

**Use**

- Captions
    
- Subtitles
    
- Accessibility
    

---

## `<iframe>`

**Purpose:** Embeds another webpage or external content.

**Use**

- YouTube videos
    
- Google Maps
    
- Documents
    
- External websites
    

⭐ Most commonly used multimedia tag.

---

## `<embed>`

**Purpose:** Embeds external files or plugins.

**Use**

- PDFs
    
- SVGs
    
- External media
    

⚠️ Used less often today. Prefer more specific elements (`<video>`, `<audio>`, `<iframe>`) when possible.

---

# ⭐ Most Used

- `<video>`
    
- `<audio>`
    
- `<source>`
    
- `<iframe>`
    

---

# ⭐ Occasionally Used

- `<track>`
    
- `<embed>`
    

---

# ✅ Best Practices

- Always use the `controls` attribute for audio and video.
    
- Use multiple `<source>` elements for better browser compatibility when needed.
    
- Add `<track>` for captions to improve accessibility.
    
- Use `<iframe>` only for trusted external content.
    
- Prefer modern HTML elements over `<embed>` where possible.