# Shared Project Footer (CNJM)

A shared HTML footer snippet for CNJM student projects. It provides a consistent, centrally managed footer via an `<iframe>`.

---

## Integration

Place this snippet where the footer should appear. The `id` is required for styling.

```html
<iframe
  id="footer-iframe"
  src="https://danieloliveira1802875.github.io/cnjm-footer/"
  title="CNJM Footer Content"
  scrolling="no">
</iframe>
```

Add the following styles to your project's stylesheet or a `<style>` block in your document's `<head>`. This CSS ensures proper layout and responsiveness.

```css
#footer-iframe {
  width: 100%;
  border: none;
  display: block;
  overflow: hidden;
  
  /* Default height for single-line view */
  height: 30px;
}

/* Adjust height for two-line view on smaller screens */
@media (max-width: 768px) {
  #footer-iframe {
    height: 60px;
  }
}
```