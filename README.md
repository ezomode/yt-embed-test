# yt-embed-test

This repo is a test page set. It tests how the YouTube IFrame API player starts in two cases.

## What it tests

The player starts in a hidden container in one page. The player starts in a visible container in the other page. The test shows if a hidden start changes the player size or state.

Each page loads the same video (`aqz-KE-bpKQ`). Each page mutes the player. Each page writes player state to a log box on the page.

## Pages

- `a-hidden.html` — The player starts inside a container with `display: none`. The page shows the container after 2 seconds. Then it loads the video.
- `b-visible.html` — The player starts in a visible container. The page loads the video at once.

## How to view a page

1. Open `a-hidden.html` or `b-visible.html` in a web browser.
2. Wait 12 seconds.
3. Read the log box on the page.
4. Compare the log text of the two pages.

## Notes

- The pages need internet access. They load the YouTube IFrame API from `youtube.com`.
- There is no build step. There are no dependencies to install.
- This repo is a test only. It is not a library or a product.
