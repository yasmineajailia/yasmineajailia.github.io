# Project Demos

Place your recording files in this directory.

Recommended formats and file names:
- `nextlearn-demo.mp4` (or `.webm`)
- `verbot-demo.mp4`
- `ats-demo.mp4`
- `prime-demo.mp4`

### How to activate a video demo in index.html:
Inside `index.html`, find the `<div class="demo-section">` for the corresponding project, and swap the placeholder with:

```html
<div class="demo-player">
  <video src="demos/nextlearn-demo.mp4" controls preload="metadata"></video>
</div>
```
