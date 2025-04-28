Bug Report: Background Color Not Displayed in TradeVeil (Lipsticks and Sunglasses page)
Describe the bug
When a custom background color is set for the lipstick and sunglasses page, the content is displayed correctly, but the specified background color is not visible. The page continues to show the default or transparent background, ignoring the custom color provided via CSS.

To Reproduce

Open the TradeVeil website.

Navigate to the lipstick and sunglasses viewer section.

Apply a custom background color to the report viewer page using CSS (e.g., background-color: 11c38b;).

Observe that the report content appears as expected, but the background color does not change.

Expected behavior
The report viewer page should display both the report content and the selected background color. The custom background color should be visible behind the report content, improving visibility and aesthetics.

Screenshots
If applicable, attach screenshots showing the report viewer with the content visible but the background color not applied.

Environment:

Browser: Firefox

Version: 22

OS: Windows 11

Additional context

The issue occurs when a custom background color is set via CSS, but the color is not rendered in the report viewer page.

The content displays properly, indicating that only the background styling is affected.

Using a more specific CSS selector (e.g., .trv-page-wrapper { background-color: red; }) may resolve the issue and allow the background color to appear as intended.

The problem may be related to CSS specificity, stacking context, or browser rendering differences.

Review recent CSS or template changes, and consider placing custom CSS directly on the page rather than within viewer templates to ensure compatibility during upgrades or template changes.

Note: Ensuring the correct selector and placement of custom CSS is crucial for the background color to display as expected without affecting the report content.
