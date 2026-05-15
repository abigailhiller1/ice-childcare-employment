# ICE enforcement and childcare employment — interactive event-study figure

Interactive companion to Figure 2 in Aslim, Currie, Herbst & Tekin (2026), *How Rising ICE Activity Influences the Childcare Workforce.*

**Live chart:** [abigailhiller1.github.io/ice-childcare-employment](https://abigailhiller1.github.io/ice-childcare-employment/)

The chart shows event-study estimates of foreign-born women's childcare employment around Trump's January 2025 inauguration, broken out by setting: any childcare, center-based, home-based, and private household. Click a setting in the legend to highlight it with its 95% confidence interval.

## Embed (recommended — auto-resizing)

This is the version to use in the Tobin brief. The iframe auto-sizes to its content on any screen width, so it behaves on mobile the same way a Datawrapper or Flourish embed does.

```html
<iframe
  id="bfi-ice-childcare"
  src="https://abigailhiller1.github.io/ice-childcare-employment/"
  width="100%"
  height="560"
  frameborder="0"
  scrolling="no"
  title="Event-study of ICE enforcement effects on foreign-born childcare employment"
  style="border: 0; width: 100%; max-width: 760px; display: block; margin: 0 auto;">
</iframe>
<script>
(function () {
  window.addEventListener("message", function (e) {
    if (!e.data || e.data.type !== "bfi-embed-height") return;
    if (e.data.id !== "ice-childcare-employment") return;
    var f = document.getElementById("bfi-ice-childcare");
    if (f && typeof e.data.height === "number") {
      f.style.height = (e.data.height + 4) + "px";
    }
  });
})();
</script>
```

## Embed (fallback — no scripts)

If the host CMS strips `<script>` tags from embeds (some content-management systems do, depending on permissions), use the iframe by itself. Height stays fixed; the chart still scales width-wise but you'll have some empty space on wide screens or possible clipping on narrow ones.

```html
<iframe
  src="https://abigailhiller1.github.io/ice-childcare-employment/"
  width="100%"
  height="600"
  frameborder="0"
  title="Event-study of ICE enforcement effects on foreign-born childcare employment"
  style="border: 0; width: 100%; max-width: 760px; display: block; margin: 0 auto;">
</iframe>
```

## Data

Estimates are loaded inline in `index.html` (the `series` array near the top of the `<script>` block). Source data: monthly Current Population Survey merged with state-level ICE apprehension records from the Deportation Data Project, September 2023 through September 2025.

To update values after a paper revision: edit `index.html` directly in the GitHub web editor, change the numbers in the `series` array, and commit. GitHub Pages redeploys automatically within a minute.

## Source

Aslim, E. G., Currie, J., Herbst, C. M., & Tekin, E. (2026). *How Rising ICE Activity Influences the Childcare Workforce.*

Prepared by the Becker Friedman Institute for Economics, University of Chicago, in partnership with the Tobin Center for Economic Policy at Yale.
