# @aliou/pi-theme-jellybeans

## 0.1.7

### Patch Changes

- c87d226: Add the Pi `scrollbarThumb` color token so fullscreen scrollbars use the theme border color.

## 0.1.6

### Patch Changes

- 29d1f59: Harmonize the thinking-level border progression across all 7 levels and add the new `thinkingMax` token.

  The Pi theme docs specify thinking borders as a "visual hierarchy from subtle to prominent." The native Pi themes implement this as a hue rotation with monotonically increasing saturation (neutral grey → blue → purple → magenta → pink).

  The previous jellybeans ladder was incoherent — hue jumped blue → brown → blue → orange across levels. This reworks the whole ladder into a single smooth warm arc that fits the jellybeans earthy identity: neutral grey → warm taupe → amber brown → gold → orange → magenta cap. Saturation ascends monotonically and hue rotates continuously through the warm spectrum, wrapping to magenta at the top (the natural end of a warm red→pink→magenta rotation, matching the native theme's magenta cap).

  New palette vars: `taupe`, `amber`, `magenta` (one value per theme variant). `thinkingLow` and `thinkingHigh` reassigned onto the arc; `thinkingMax` added.

## 0.1.5

### Patch Changes

- c34c567: Update Jellybeans mono theme metadata and palette variables for current Pi theme schema.

## 0.1.4

### Patch Changes

- f3101be: Add a package description so the published theme page can display summary text.

## 0.1.2

### Patch Changes

- b5c4cd1: Update demo video and image URLs for the Pi package browser.

## 0.1.1

### Patch Changes

- 4e0eb81: Fix screenshot URLs in README

## 0.1.0

### Minor Changes

- 0398a67: Publish Jellybeans mono themes as a Pi theme package.
