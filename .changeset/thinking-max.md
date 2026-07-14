---
"@aliou/pi-theme-jellybeans": patch
---

Harmonize the thinking-level border progression across all 7 levels and add the new `thinkingMax` token.

The Pi theme docs specify thinking borders as a "visual hierarchy from subtle to prominent." The native Pi themes implement this as a hue rotation with monotonically increasing saturation (neutral grey → blue → purple → magenta → pink).

The previous jellybeans ladder was incoherent — hue jumped blue → brown → blue → orange across levels. This reworks the whole ladder into a single smooth warm arc that fits the jellybeans earthy identity: neutral grey → warm taupe → amber brown → gold → orange → magenta cap. Saturation ascends monotonically and hue rotates continuously through the warm spectrum, wrapping to magenta at the top (the natural end of a warm red→pink→magenta rotation, matching the native theme's magenta cap).

New palette vars: `taupe`, `amber`, `magenta` (one value per theme variant). `thinkingLow` and `thinkingHigh` reassigned onto the arc; `thinkingMax` added.
