# Write alt text for images missing it

**Area:** On-page optimization · **Time:** 45 min · **Skill:** `image-alt-batch`

**Goal.** Give every image on your traffic pages a specific alt text that describes what is in it and serves the page's topic.

**When.** A crawl reports hundreds of images with missing or empty alt attributes.

## You need

- a crawler images export with image URL, the page it sits on, and the alt text column
- for each image, the filename, the caption or the surrounding paragraph, or the image itself if you can upload it
- a 28-day Search Console Pages export to prioritise pages by impressions

## Steps

1. Filter the images export to rows with empty alt, join it to the Pages export on the page URL, and sort by the page's impressions so the busiest pages come first.
2. For the top 50 images, collect the filename, the caption if any and the paragraph around each, or upload the image files to Claude in batches of 10.
3. Ask Claude to write one alt text per image under 125 characters that says what the image shows, and to write decorative for images that carry no information.
4. Claude returns image URL, page URL, alt text or decorative, and flags any image it could not describe from the material given.
5. Paste the alt texts into the CMS, set the flagged ones after looking at the image yourself, and set decorative images to an empty alt attribute.

**Done when the top 50 images by page impressions have a specific alt text or an intentional empty alt attribute live.**

## Rules

- Claude never states a number it was not given. It writes "cannot compute from this data" instead of estimating.
- Every step ends on one action, not a list of options.
