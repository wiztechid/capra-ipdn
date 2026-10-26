# CAPRA Article Share Standard — Frozen v1

Status: FROZEN for every editorial article published on Web CAPRA IPDN.
Effective: 26 October 2026.

## Required placement

Every article page has exactly two share bars using the same component:

1. Immediately below the article hero image.
2. At the end of article content, after the editorial verification note and before the article closes.

Do not add share bars to the homepage, legal pages, or contact/about utility pages.

## Buttons and behavior

Use the same order, labels, and colors on every article:

- WhatsApp — green
- Telegram — light blue
- Facebook — blue
- Salin link — light gray with dark text

Social destinations must be built from the page's current URL and title at runtime, so canonical page links are shared without query or route mistakes. The copy button must copy the current article URL, announce success to screen readers, show a temporary “Tersalin” state, and provide a manual fallback message if clipboard access is unavailable.

The component uses `capra-share`, `data-share`, and `data-copy-share` selectors. The same script must initialize every matching button on the page, including both share bars.

## Visual and accessibility requirements

- Rounded, high-contrast buttons with visible keyboard focus.
- Responsive layout: two columns on narrow screens; rows can wrap on wider screens.
- Use an accessible region label and a polite live region for copy feedback.
- Keep the bar within the article content width and preserve existing article layout.
- Add safe `rel="noopener noreferrer"` to social links opened in a new tab.
- Avoid duplicate share bars or legacy duplicate copy handlers.

## Change control

This standard is frozen. Apply it unchanged when creating or updating article pages. Any proposed change to button order, labels, colors, placement, or behavior requires an explicit template revision; article content edits do not alter this standard.
