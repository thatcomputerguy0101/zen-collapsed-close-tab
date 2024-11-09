# Zen Collapsed Close Tab

This mod for [Zen Browser](https://zen-browser.app) shows closed tab buttons when hovering over tabs when the tab bar is collapsed. It works with the tab bar on either side of the window.

![Demo collapsed sidebar with visible close button on a tab](demo.png)

## Installation (Not yet available on the store)

1. Open https://zen-browser.app/mods in the Zen Browser
2. Search for "Collapsed Close Tab"
3. Click "Install Theme"

### Manual Installation

1. Create `userChrome.css` as described at https://docs.zen-browser.app/guides/live-editing
2. Copy the contents of `chrome.css` from this repository into the newly created `userChrome.css`
3. Relaunch Zen Browser if necessary to apply the theme

## Quirks

The scrollbar for tabs appears on the outside edge of the window, instead of always appearing on the right edge. This is so that tabs can extend over the content area when hovered over.

This mod was confirmed to be compatible with the built-in color themes, but user-installed themes may cause unexpected tab colors. The background under hovered tabs may appear strange if the tab bar background is not a solid color.

This relies on a niche CSS bug to set the `pointer-events` style on the correct elements, and therefore is at (low) risk of being unable to interact with the scrollable portion of the tab bar at some point in the future.
