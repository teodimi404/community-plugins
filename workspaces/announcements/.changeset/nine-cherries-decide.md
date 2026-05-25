---
'@backstage-community/plugin-announcements': patch
---

Fixed announcement form prefilling the end date with today + 7 days, which silently set an until_date on announcements that were meant to be open-ended. The field now starts empty for both new and edited announcements, and empty values are submitted as undefined.
