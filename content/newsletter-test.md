---
title: "Newsletter Integration Test"
date: 2024-01-15
type: page
---

# Newsletter Integration Test

This page tests the newsletter integration with your beehiiv URL: `https://newsletter.shiftelevate.dev`

## Simple Newsletter Link

[Visit my newsletter →](https://newsletter.shiftelevate.dev?utm_source=website&utm_medium=newsletter&utm_campaign=test&utm_content=test_page)

## Direct Link Test

[Direct newsletter link](https://newsletter.shiftelevate.dev?utm_source=website&utm_medium=newsletter&utm_campaign=test&utm_content=direct_link)

## Analytics Events to Check

When you click the newsletter links above, you should see these events in Google Analytics:

1. `newsletter_click` - For newsletter link clicks
2. UTM parameters should be: `utm_source=website&utm_medium=newsletter&utm_campaign=test&utm_content=test_page`

## Expected UTM Parameters

- **utm_source**: `website`
- **utm_medium**: `newsletter` 
- **utm_campaign**: `test` (or `main` for default)
- **utm_content**: `test_page` (location-specific)
