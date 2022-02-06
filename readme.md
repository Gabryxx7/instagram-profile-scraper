# Instagram Profile Scraper
## Features
- Scrape data from your own profile or any public profile
- Safe (uses your own cookies)
- Extract data from Instagram Data Export (Can request one here: [https://www.instagram.com/download/request/](https://www.instagram.com/download/request/))
- Can be scheduled to run every day and update your own website gallery/instagram feed
- Downloads high quality post images, captions and metadata

## Instructions
### Get cookies and `query_hash`
In order to avoid being blacklisted as a bot, the best way to set up the bot is to get your cookies and `query_hash` from your own browser.
The process is rather easy!
1. Navigate to [https://www.instagram.com(https://www.instagram.com)
2. Open the Developer Tools (on Chrome is `f12` or `CMD + OPTION + i`)
3. In the developer tools window, open the "Network" tab
4. Login and navigate to your own profile page
5. Scroll down enough to load the next posts in your timeline
6. In the Filter textbox (top left in the Network tab), type `query_hash` and click on the list element
8. From the right side, click on "Headers"
9. Look for `cookie` in the list, then right-click -> copy value
10. Go to the "Payload" tab, just next to the "Headers" one
11. Look for `query_hash` then right-click -> copy value
12. Add these two to your `insta_config.yaml` file and you're set :)

### Scrape Profile Data
- Start by editing `insta_config.yaml` to add
