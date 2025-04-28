# Pull Request

## Description
Fixes an issue where a custom background color was not displaying on the Lipsticks and Sunglasses pages of the TradeVeil website. The content appeared correctly, but the background color remained default/transparent even after applying custom CSS. This fix ensures that the background color renders properly by enhancing CSS specificity.

## Type of change
- [x] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Checklist
- [x] I have tested my code locally.
- [x] I have added necessary documentation if needed.
- [x] I have assigned reviewers.

## Linked Issues
Closes # (Background Color Not Displayed in TradeVeil - Lipsticks and Sunglasses page)

## Bug Report Summary

**Describe the bug**  
When a custom background color is set for the Lipsticks and Sunglasses pages, the content displays properly, but the specified background color does not appear. The page continues to show a transparent or default background.

**To Reproduce**  
1. Open the TradeVeil website.
2. Navigate to the Lipsticks or Sunglasses viewer page.
3. Apply a custom CSS background color (e.g., `background-color: #11c38b;`).
4. Notice that the content is visible but the background color is not applied.

**Expected behavior**  
The custom background color should appear behind the report content, enhancing visibility and user experience.

**Environment**  
- Browser: Firefox
- Version: 22
- OS: Windows 11

**Additional Context**  
The issue may be caused by CSS specificity problems or stacking contexts. Fixing it involves using a more specific selector, such as `.trv-page-wrapper { background-color: red; }`, and ensuring styles are applied outside viewer templates to maintain compatibility through upgrades.

