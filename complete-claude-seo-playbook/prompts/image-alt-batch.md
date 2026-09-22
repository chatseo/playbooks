# Write alt text for a batch of images

**Area:** On-page optimization

**When.** Paste this with an image list when a crawl shows missing or keyword stuffed alt attributes.

## Prompt

```
Below is a list of images: each row has the filename, the page URL, the nearest heading, and the current alt text (blank if none). If the list is missing page context, ask me for it before doing anything.

Write one alt text per image, 4 to 16 words, describing the image for someone who cannot see it, naming the subject specifically (the product, the chart, the screen), and using the page's topic term only where the image actually shows it. Rules: no "image of" or "picture of", no keyword lists, decorative images (dividers, icons) get an empty alt marked decorative, charts state their finding, screenshots name the tool and the screen. Do not guess what an image shows: if the filename and context do not tell you, write "needs a look". If a number is not in the data I gave you, write "cannot compute from this data". Never estimate.

Output a table, max 30 rows, columns: image, page, current alt, new alt, type (content, chart, screenshot, decorative, needs a look).

Finish with one action: the one image to fix first, no alternatives.
```
