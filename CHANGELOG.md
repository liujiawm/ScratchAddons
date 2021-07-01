# Changelog

All notable changes to this project will be documented in this file.

**Note:** This changelog is more detailed, compared to the summarised changelog on https://scratchaddons.com/changelog.

<!-- 

# Note:

- Every changes related to the addon are required to be added, except meta changes such as README, CI, etc.
- Use the compare feature to know the difference between each version. (eq. https://github.com/ScratchAddons/ScratchAddons/compare/v1.10.0...v1.11.0).
- Verify the content of the PR/commit. Write it differently if needed.
- Seperate each addon if changes are across multiple addons.
- Use the name of the addon based on the latest commit on the version. (https://scratchaddons.com/addons)
- If a version is yanked, keep the changes below the yanked version. DO NOT MERGE it to the next version.
- Check the bottom of this file for resources.
- Avoid including priority of a change. (for now)
- Addon-specific changes should be started with the addon name, followed by a colon, and then the change.
- Additions and removals changes should be written as a noun phrase. Others are sentences.

# TODO list:

- Changed entries on "Fixed" section into "Fix ..." sentence form (noun phrase) (v1.4.1 - v1.13.0)
- Verify changelog contents (v1.4.1 - latest)
- Complete missing changelog (v1.2.0)
- Add new languages on localization (v1.4.1 - latest)

-->

## [v1.16.3] - 2021-06-20

### Fixed

#### Addons

- Scratch Messaging: Fix link color on light mode (#2843)

## [v1.16.2] - 2021-05-19

### Added

#### Addons

- Scratch Messaging: Support for new emojis (#2828)
- Scratch Notifier: Support for new emojis (#2828)
- Show ocular.jeffalo.net statuses and post reactions: Reacting to post using keyboards (#2824)
- Studio manager tools: Support manager limit (#2817)

### Changed

#### Addons

- Studio manager tools: Mark as beta addon (#2835)

### Fixed

#### Addons

- Better forums post editor buttons: Show posted images (#2812)
- Copy link to comment button: Fix button disappearing when loading older comments (#2831)
- Debugger: Fix window cannot be moved when partially hidden (#2804)
- Debugger: Fix blocks do not run when on a sprite not selected after reload (#2804)
- Debugger: Fix addon sometimes does not work when going inside the editor (#2804)
- Debugger: Fix addon when "going to" block not working immediately after leaving editor and returning to editor
- Debugger: Improve performance of logging items by ~100x  (#2804)
- Debugger: Fix unread logs icon not appearing reliably when items are being logged (#2804)
- Debugger: Activate the code tab when going to a block (#2804) 
- Debugger: Fix bug when custom blocks can't be deleted (#2819)
- Debugger: Don't show "Edit" when right clicking on an addon block (#2819)
- Scratch Messaging: Fix broken link by mentions by using raw ref for relative path rewriting (#2816)
- Scratch Messaging: Fix prompt of users to log in appearing when a comment was deleted (#2806)
- Scratch Messaging: Make links an actual link instead of using events (#2813)
- Show ocular.jeffalo.net statuses and post reactions: Move reaction tooltips in front of reaction menu (#2802)
- Show ocular.jeffalo.net statuses and post reactions: Fix reaction menu not being centered when post has no reactions (#2802)
- Website dark mode: Fix addon does not make remix tree dark (#2836)

#### Extension and Addon API

- Move `handleKeySettings` to addon-settings component to make the Settings page faster (#2803)
- Fix bug where disabled addons stay in the search result after clearing search bar in popup settings (#2830)

## [v1.16.1] - 2021-05-15

### Fixed

#### Addons

- Debugger: Fix addon logging empty string if sprite is not focused (#2775)
- Debugger: Change how the block "previews" are generated to not rely on an actual Blockly block existing (#2775)
- Debugger: Don't try to scroll a block in a flyout into view (#2775)
- Debugger: Make the button not disappear when entering and leaving fullscreen (#2775)

## [v1.16.0] - 2021-06-14

### Added

#### Addons

- Debugger (#2161)
- Expandable search bar (#2619)
- Redirect mobile forums to main forums (#2667)
- Editor dark mode and customizable colors: Add settings for darkening monitors (#2699)
- Editor dark mode and customizable colors: Add boolean setting (#2699)
- Editor dark mode and customizable colors: Add a setting to change the color of blue text and icons (#2699)
- Gamepad support: Analyze the project's scripts and try to generate decent mappings by default (#2658)
- Gamepad support: Allow project creators to set mappings (#2658)
- Gamepad support: Allow configuring the keys of each axis individually (#2658)
- Gamepad support: Allow binding button to Enter key (#2658)
- Scratch 2.0 → 3.0: Support for migrated studio (#2661)
- Website dark mode: Support for migrated studio (#2661)

#### Extension and Addon API

- Fuzzy searching in Settings page (#2705)
- Prioritization on some fields searching Settings page (#2705)
- Icons to external links on Settings page (#2724)

### Changed

#### Addons

- Editor dark mode and customizable colors: Replace the editor dark mode userscript with customCssVariables to set the values (#2651)
- Editor dark mode and customizable colors: Make the block palette affected by the border color setting (#2651)
- Editor dark mode and customizable colors: Make inactive tab icons brighter when the background is dark to match the text color (#2651)
- Gamepad support: Hide Gamepad support config button in small stage mode (#2658)
- Gamepad support: Hide real mouse cursor when virtual cursor is being used (#2658)
- Gamepad support: Close settings when escape is pressed (#2658)
- Scratch Messaging: Linkify mentions and URLs (#2700)
- Show ocular.jeffalo.net statuses and post reactions: Update reactions UI (#2704)

#### Extension and Addon API

- Optimize the settings page for relevance-ordered search (#2650)

### Fixed

#### Addons

- Clone counter: Fix addon not hiding when dynamically enabled in a small stage editor (#2683)
- Clone counter: Fix addon not appearing when going inside the editor (#2694)
- Custom block shape: Fix offsets being added to small reporter blocks (#2623)
- Developer tools: Ignore Ctrl+Shift+F (#2746)
- Discuss button: Fix addon not enforcing minimum or maximum label length (#2687)
- Do not automatically run duplicated blocks: Fix addon not working if a duplicated block is dropped in an input (#2625)
- Editor dark mode and customizable colors: Make the text on hovered inactive tabs transparent to match Scratch design (#2625)
- Editor dark mode and customizable colors: Style modal back and close icons correctly (#2651)
- Editor dark mode and customizable colors: Fix sound icon of the selected sound using `selector2-filter` instead of the correct `selectorSelection-filter` (#2651)
- Editor dark mode and customizable colors: Make the selection background and handles in the sound editor affected by the highlight color setting (#2699)
- Editor dark mode and customizable colors: Removes unused camera modal styles (#2699)
- Feature unshared projects Do not polute XHR.open to make it reliable (#2748)
- Filter messages on Scratch's messages page: Fix addon hides unread messages (#2733)
- Forum search: Escape external HTML before insertion (#2684)
- Gamepad support: Change category to "Project player" instead of "Other" (#2658)
- Gamepad support: Fix addon not hiding when dynamically enabled in a small stage editor (#2683)
- Mouse position: Fix addon not hiding when entering a small stage editor (#2683)
- Mouse position: Fix addon not hiding in small stage editor if Gamepad support is enabled (#2683)
- Mouse position: Fix addon not hiding when dynamically enabled in a small stage editor (#2683)
- Scratch Messaging: Apply min-height instead of height to avoid bottom bar being overflow (#2685)
- Scratch Messaging: Handle errors to avoid addon crashing when Scratch is down (#2759)
- Show exact count: Fix addon adding project count instead of replacing existing ones (#2661)
- Website dark mode: Fix unreadable crash messages (#2706)
- Website dark mode: Fix unreadable email confirmation modal (#2721)

#### Extension and Addon API

- Fix userscripts being executed twice on the same page (#2680)
- Fix long addon names in settings taking unnecessary space (#2688)
- Fix wrapping on tag badges in settings (#2688)
- Do not enforce maximum width for addon descriptions (#2688)
- Fix text color on More Settings (#2691)
- Fix grammar on forum warning message (#2723)

## [v1.15.0] - 2021-05-25

### Added

#### Addons

- Filter messages on Scratch's messages page (#1704)
- Block transparency (#2332)
- Do not automatically run duplicated blocks (#2470)
- Ctrl+Click to run scripts (#2555)
- Confirm actions: Support for confirming closing topics (#2455)
- Gamepad support: Support for WASD key mapping (#2541)
- Gamepad support: Allow setting buttons to be hidden when disconnected (#2541)
- Message count on extension icon: Allow changing the badge color (#2430)
- More links: Support for linkifying migrated studio descriptions (#2560)
- Scratch 2.0 → 3.0: Support for migrated studios (#2584)
- Scratch Messaging: Support for messages from Scratch Team (#2431)
- Scratch Messaging: Explanation to why a comment could not be posted (#2569)
- Website dark mode: Support for migrated studios (#2584)

#### Extension and Addon API

- RTL support (#2263)

### Fixed

#### Addons

- Thumbnails setter: Fix addon running when logged out (#2174)
- Shared/edited dates tooltip: Fix addon erroring when logged out (#2174)
- Better forums post editor buttons: Fix addon causes forum emojis to disappear (#2437)
- Confirm actions: Fix addon triggering when clicking "Shared" on shared projects (#2441)
- Developer tools: Fix find bar not working with cross-sprite broadcasts (#2474)
- Developer tools: Fix addon triggering "paste" action when it shouldn't in Linux (#2474)
- Developer tools: Fix palette showing at the wrong place (#2474)
- Developer tools: Fix addon not showing palette after using custom block modal (#2474)
- Developer tools: Fix addon not allowing palette text input to be interacted with mouse (#2474)
- Data category tweaks: Use Blocky to fix addon not working sometimes (#2528)
- Gamepad support mouse: Fix virtual mouse cursor bugs on high DPI/retina displays (#2541)
- True forums YouTube links: degrades performance on all Scratch pages (#2547)
- Studio manager tools: Fix incompatibility with "Website dark mod"e when styling buttons for migrated studios (#2584)
- Studio manager tools: Fix addon duplicating tabs in migrated studios (#2589)

#### Extension and Addon API

- Color picker in settings causes lag (#2370)
- Scratch Addons silently breaks when using old browsers (#2518)
- Addon descriptions on settings have wrong color on light mode (#2556)
- Settings page take too long to load (#2567)
- Scratch Addons does not run on startup-loaded tabs (#2574)
- Failure to post a project comment crashes the page (#2592)
- Color picker opacity slider and input in settings are always hidden (#2597)
- Settings page cause crashes in older Firefox (#2605)

## [v1.14.3] - 2021-05-15

### Added

#### Addons

- Support for new studio page 
	- Scratch 2.0 → 3.0 (#2485)
	- Website dark mode (#2485)
	- Show exact count (#2492)
	- Infinite scrolling (#2493)
	- Studio manager tools (#2493)
	- Linebreaks in comments (#2493)
	- Confirm actions (#2493)
	- Copy link to comment button (#2493)
	- More links (#2493)
	- Resizable comment input (#2496)

#### Extension and Addon API

- Support of new studio comments in mute prevention code (#2486)

### Changed

#### Addons

- Switch Scratch Messaging to use new APIs (#2501)

### Fixed

#### Addons

- Cloud games: Fix user icon being white (#2461)
- Disallow and remove use of Event.path to avoid errors when clicking on profile pages in Firefox (#2477)

### Removed

#### Extension and Addon APIs

- Remove unfinished translations (#2472)

## [v1.14.2] - 2021-05-09

### Fixed

#### Addons

- Remix tree button: Fix button getting added on project pages to unshared projects (#2436)
- Shared/edited dates tooltip: Fix addon causes unshared projects to not load (#2454)
- Show ocular.jeffalo.net statuses and post reactions: Fix reactions not styled properly (#2408)
- Show ocular.jeffalo.net statuses and post reactions: Change reference of "my-ocular" to "ocular" (#2428)
- Make addons run on error pages (#2416)

#### Extension and Addon API

- Fix arrow above the popup on Firefox that is black regardless of the theme setting (#2405)
- Fix some addons crashing when Redux is unavailable (#2420)

## [v1.14.1] - 2021-05-05

### Fixed

#### Addons

- Fix reduxEvents regressions that causes some addons not running (#2385)

## [v1.14.0] - 2021-05-05

### Added

#### Addons

- Better forums post editor buttons (#2081)
- Editor sound effects (#2254)
- Gamepad support (#2149)
- Remove curved stage border (#2286)
- Customizable block colors: Dark presets (#2207)
- More tags to addons (#2326)

#### Extension and Addon API

- Prevent users from commenting "Scratch Addons" (#2212)
- Addon groups and subcategories (#2260)

### Changed

#### Addons

- Cat blocks: Show as normal addons (#2251)
- Customizable block colors: Change setting names to avoid confusion (#2241)
- Drag and drop files: Mention new features on description (#2234)
- Editor dark mode: Change setting names to avoid confusion (#2241)
- Show exact count: Do not ping external servers on default setting (#2326)
- Show ocular.jeffalo.net statuses and post reactions: Change addon name from "Show my-ocular status" (#2163)
- Reduce addon operations on DOM changes (#2268)

#### Extension and Addon API

- Update all settings at once when loading presets (#2278)

### Fixed

#### Addons

- Custom scripts area zoom settings: Fix addon miscalculates zoom (#2309)
- Customizable block colors: Affect block dropdown borders (#2207)
- Customizable block colors: Fix incompatibility with Developer tools (#2207)
- Customizable block colors: Fix addon affects stage monitors and ask prompts (#2241)
- Developer tools: Fix incompatibility with Customizable block colors (#2148)
- Developer tools: Fix typos on help message (#2259)
- Developer tools: Fix addon uses wrong message in help (#2259)
- Developer tools: Fix addon not follow capitalization rules (#2280)
- Display stage on left side: rounds the corners (#2245)
- Editor dark mode: Fix addon affects stage monitors and ask prompts (#2241)
- Use local timezone: Fix addon does not translate "yesterday" and "today" on forums (#2214)

#### Extension and Addon API

- Fix themes show "for editor" tags in "All" mode on settings page (#2260)
- Fix color pickers of disabled addons' settings can be opened (#2260)
- Fix reset button showing on disabled addons' settings (#2260)
- Fix disabled buttons changing style when hovered (#2260)
- Fix popup incorrectly sized in Firefox when opened from overflow menu (#2274)
- Fix "View Changelog" in update notification incorrectly capitalized in some languages (#2279)
- Fix color pickers in settings can't be closed by clicking (#2315)
- Fix color pickers in settings cap brightness at 99% (#2323)
- Fix bug when isabling an addon without userscripts causes other addons to appear as disabled (#2340)
- Fix bug when enabling an addon causes the addon to appear as running on all pages (#2341)

### Removed

#### Addons

- Project screen reader support (#2282)
- Developer tools: Remove referrence to griffpatch (#2259)

## [v1.13.0] - 2021-04-20

### Added

#### Addons

- Change new sprite default position (#2116)
- Custom scripts area zoom settings (#2034)
- Save blocks as image (#2087)
- Developer tools: Ability to disable certain features (#2146)
- Drag and drop files: Support for dropping text files (#2013)
- Shared/edited dates tooltip: Tooltip for shared date (#1940)
- Website dark mode: Support for "become a scratcher" notice (#2167)
- Website dark mode: Support for embedded projects (#2042)
- Website dark mode: Support for profile text placeholders (#2051)
- Website dark mode: Support for statistics (#2037)

#### Extension and Addon API

- User agent modifying (#1920)
- Ability to enable addons without refreshing (#1961)
	- `addon.self.enabledLate` property
	- `disabled` event
	- `reenabled` event
	- `dynamicEnable` manifest property
	- `injectAsStyleElt` manifest property
	- `updateUserstylesOnSettingsChange` manifest property
	- `data-sa-hide-if-disabled` attribute

### Changed

#### Addons


- Developer tools: Enable by default (#2146)
- Developer tools: Set color for event blocks, ignoring "Customizable block colors" addon (#2146)
- Editor dark mode and customizable colors: Change name from "Editor dark mode" (#1805)
- Editor dark mode and customizable colors: Use presets (#1805)
- Highlight currently executing blocks: Improve highlighting (#1956)
- Highlight currently executing blocks: Improve performance by not calling querySelectorAll 30 times per second (#2178)
- Shared/edited dates tooltip: Rename addon from "Shared/edited dates tooltip" (#1940)

#### Extension and Addon API

- Move `sourceURL` and `%addon-self-dir%` to be evaluated in the background page (#1961)
- Speed up loading of settings page (#2191)
- Stringify integer settings (#2142)
- Update localization strings

### Fixed

#### Addons

- Alt+GreenFlag 60FPS player mode: Fix alt key being detected when it is not pressing on ChromeOS (#2184)
- Cat blocks: Fix ears not showing in Firefox (#2145)
- Cat blocks: Fix incompatibiity with other addons (#2210)
- Cat blocks: Fix texts overflowing the hat blocks (#2147)
- Forums image uploader: Fix incompatibility with "Website dark mode" addon (#2056)
- Highlight currently executing blocks: Step VM before displaying running scripts to fix 1 frame lag (#2178)
- Live featured project: Disable scrollbar (#2118)
- Mute project player: Fix control key detection (#2098)
- Scratch 2.0 → 3.0: Scrollbars on studio descriptions got disabled (#2137)
- Sprite folders: Fix improper handling backpacking of sound folders (#2103)
- Studio manager tools: Fix addon not allowing managers to leave studios (#2199)
- Variable manager: Fix addon not handle renaming variables to have duplicates (#2160)
- Variable manager: Fix addon not load when re-entering the editor (#2160)
- Website dark mode: Fix incorrect border color (#2051)

#### Extension and Addon API

- Fix crash when opening editor from My Stuff on Firefox (#2209)

### Removed

#### Extension and Addon API

- `/* sa-autoupdate-theme-ignore */` (#1961)

## [v1.12.1] - 2021-04-01

### Changed

#### Extension and Addon API

- Update localization strings

### Fixed

#### Addons

- 2D color picker: Addon breaks on Firefox (#2004)
- Alt+GreenFlag 60FPS player mode: Typo at notice (#2021)
- Auto-hide block palette: Lock icon placed at the wrong place (#2011)
- Auto-hide block palette: Re-entering the editor if category click mode is used breaks addon. (#2011)
- Auto-hide block palette: Wrong lock icon shown after re-entering the editor (#2011)
- Auto-hide block palette: Changing "toggle on" setting while in use crashes addon (#2011)
- Profile page banner: Addon breaks follow button and changes featured projects (#2014)
- Profile statistics: Incorrect chart (#2016)
- Sprite folders: Dragging a folder into empty backpack crashes addon (#2036)

## [v1.12.0] - 2021-03-28

### Added

#### Addons

- 2D color picker (#1768)
- Custom block shape (#1773)
- Dango rain on profiles (April Fools Day) (#1931)
- Drag and drop files (#1916)
- Profile page banner: Blur setting (#1889)
- Profile statistics: Message when ScratchDB is down (#1830)
- Scratch Messaging: Zaglo protection (#1912)
- Show full areas: Support for scratchblocks scroll (#1831)
- Sprite folders: Folder backpacking (#1947)
- Variable manager: Variable renaming (#1951)

#### Extension and Addon API

- `allowTransparency` property on manifest (#1781)
- Transparency on settings page color picker (#1781)

### Changed

#### Addons

- Profile page banner: Use higher resolution (#1889)

#### Extension and Addon API

- Update localization strings

### Fixed

#### Addons

- Auto-hide block palette: Broken animation (#1980)
- Developer tools: Inconsistent capitalization on context menu (#1919)
- Developer tools: "Send to top" button being added on unintended places (#1919)
- Mute project player: Can't mute on macOS (#1925)
- Profile statistics: Old API being used for follower history (#1955)

## [v1.11.2] - 2021-03-17

### Fixed

#### Addons

- Sprite folders: Editor crashing when trying to drag and drop a sound within a folder to another sprite (#1893)
- Profile statistics: Missing thousand separator comma on "most loved by country" statistic (#1894)

## [v1.11.1] - 2021-03-14

### Changed

#### Addons

- Thumbnails setter: Rename setting "Prevent thumbnail from being overwritten" to "Don't set thumbnails automatically" to avoid confusion (#1851)

#### Extension and Addon API

- Move Portuguese localization to Portuguese Brazil (#1778)
- Update localization strings

### Fixed

#### Addons

- Block palette category icons: Typo in addon name (#1786)
- Developer tools: "Clean up blocks" choice not removed from context menu (#1852)
- Disable auto-save: Revamp addon to fix manual saving (#1741, #1850)
- Editor dark mode: Scrolling not working on code area (#1849)
- Forum search: Extremely slow performance (#1826)
- Higher character limit in "What I'm Working On": Errors on other people's profiles (#1815)
- Mute project player: Mute audio engine instead of suspending so sound blocks won't stuck (#1803)
- Mute project player: Mute icon disappearing when entering/leaving editor while muted (#1803)
- Onion skinning: Incompability with "Folders" addon (#1784)
- Show exact count: Incompability with "Profile statistics" addon (#1827)
- Sprite folders: Empty-name sprites inside folders not handled properly (#1812)
- Variable manager: Broadcasts appearing (#1770)
- Variable manager: Typo (#1786)
- Website dark mode: Scrollbars don't change color on hover (#1767)

#### Extension and Addon API

- Userstyle-only addons not listed as running (#1753)

### Removed

#### Addons

- Auto-show editor extensions: Video sensing option (#1799)
- Variable manager: Feedback button (#1847)

## [v1.11.0] - 2021-03-08

### Added

#### Addons

- Block pallette category icons (#1689)
- Cloud games (#1497)
- Higher character limit in "What I'm Working On" (#1674)
- Profile statistics (#1614)
- Variable manager (#1615)
- Cloud games: Add loading indicator (#1667)
- Forums image uploader: Add more strings to localize (#1688)

### Changed

#### Addons

- Alt+GreenFlag 60FPS player mode: Change name from "60FPS player mode" for clarity (#1684)

#### Extension and Addon API

- Use HTTPS link to the contributor page (#1688)

### Fixed

#### Addons

- Auto-show editor extensions: Video Sensing is being loaded by default, causing lag (#1738)
- Block switching: Input type of variable blocks is not updating (#1731)
- Cat blocks: Addon not localized due to falsy value on manifest (#1722)
- Forums image uploader: Add more strings to translate (#1688)
- Infinite scrolling: Addon does not run on pages without trailing slash (#1712)
- Infinite scrolling: Addon makes links to project comment point to unintended part of page (#1712)
- More links: URLs with percent signs not linking (#1698)
- Profile page banner: Addon not localized due to falsy value on manifest (#1722)
- Semicolon glitch: Addon not localized due to falsy value on manifest (#1722)
- Website dark mode: Incompatibility with Infinite scrolling (#1725)

#### Extension and Addon API

- License page cannot be scrolled (#1666)
- Incorrect styles are applied to addons that load too early (#1690)
- Update localization strings

### Removed

#### Extension and Addon API

- Some dead code (#1688)
- `Addon.fetch` code (#1688)

## [v1.10.0] - 2021-02-22

### Added

#### Addons

- Auto-show editor extensions (#1568)
- Copy link to comment button (#1502)

### Changed

#### Extension and Addon API

- Addons can be searched using ID (#1597)
- Update localization strings

### Fixed

#### Addons

- Cat blocks: Extra space not added in block palette (#1623)
- Developer tools: Highlighting conflicts with editor-theme3 (#1563)
- Editor dark mode: Monitor names made invisible (#1606)
- Forums image uploader: Addon tries to run on pages without post form (#1608)
- Infinite scrolling: Incompability with "Scratch 2.0 → 3.0" addon (#1602)
- Pause button: Stack timer blocks incorrectly paused (#1555)
- Pause button: Edge-activated blocks with obscured shadows incorrectly paused (#1555)
- Pause button: Addon not resuming old threads if the user starts a new thread while paused (#1555)
- Pause button: "when sprite clicked" and "when key pressed' events should not be fired when paused (#1555)
- Pause button: Addon breaks when sa-pause block is executed when paused (#1555)
- Record project video: Addon breaks when the user exits editor view (#1571)
- Scratch Messaging: Asterisks added to links to ST members (#1585)
- Website dark mode: Addon does not make crash screen dark (#1570)
- Website dark mode: Studio follower counts made invisible (#1583)
- Website dark mode: Addon does not make popups dark (#1612)

#### Extension and Addon API

- Addons with permission requirements cannot be enabled for the first time (#1616)

## [v1.9.3] - 2021-02-15

### Fixed

#### Extension and Addon API

- Extension crashing on browsers with Spanish language (#1529)

## [v1.9.2] - 2021-02-13

### Changed

#### Extension and Addon API

- Update localization strings

### Fixed

#### Addons

- Curator link: Addon crashes on default locale (#1560)
- Display stage on left side: Direction picker partially hidden (#1549)
- Linebreaks in comments: Empty lines left on replies to ST members' comments (#1567)
- More links: Numbers and hyphens in non-IDN TLDs treated as links due to faulty regex (#1540)
- Thumbnails setter: Addons warns thumbnail is too big when the server is down (#1551)

#### Extension and Addon API

- Muted extension shows badge on refresh (#1541)
- Language codes with uppercase letters don't load (#1543)
- Extension still crashing on browsers with languages other than Englsh (#1569)

## [v1.9.1] - 2021-02-09

NOTE: All updates from [v1.9.0] are pushed on this version.

### Fixed

#### Extension and Addon API

- Extension crashing on browsers with languages other than Englsh (#1529)

## [v1.9.0] - 2021-02-08 [YANKED]

NOTE: v1.9.0 is only released on Firefox due to a bug that would make the extension crash if browser language not set to English. All updates are included on [v1.9.1].

### Added

#### Addons

- New addon: Fix capitalization of Account Settings (#1413)
- New addon: Show BBCode (#1411)
- Auto-hide block palette: "Hover in category" setting (#1419)
- Mute project player: Icon for muted projects (#1412)
- Record project video: Record mic option (#1492)
- Scratch Messaging: Support for manager promotion notifications (#1471)
- Scratch Notifier: Support for manager promotion notifications (#1471)

### Changed

#### Addons

- Developer tools: Improve UI (#1433)
- Scratch Messaging: Show usernames of lovers and favers (#1474)

#### Extension and Addon API

- Ignore shift-click on settings toggle (#1484)
- Update localization strings

### Fixed

#### Addons

- Clone counter: Addon blocks main thread (#1473)
- Developer tools: Middle click feature does not list all broadcast block options (#1390)
- Developer tools: Dropdown is not sorted (#1390)
- Developer tools: Wrong color for lists (#1390)
- Developer tools: Invalid blocks sometimes added (#1498)
- Linebreaks in comments: Space after asterisk for ST member replies (#1461)
- Linebreaks in comments: Linebreaks not preserved in some cases (#1461)
- Thumbnails setter: Addon silently fails when thumbnail server errors (#1522)
- Website dark mode: Addon does not apply to post editing pages (#1481)

#### Extension and Addon API

- Inconsistent padding in More Settings (#1418)

## [v1.8.1] - 2021-01-29

### Changed

- Make some classes not use hardcoded hashes (#1403)
- Fix unused vars and return values
- Update localization strings

### Fixed

- Auto-hide block palette: Addon causing reporter return value bubbles to remain on screen
- More links: Words with ellipsis treated as links due to faulty regex (#1416)
- Scratch 2.0 → 3.0: Gray text shown on page load by default (#1417)
- Website dark mode: Forums image uploader text unreadable (#1389)

## [v1.8.0] - 2021-01-25

### Added

#### Addons

- Disable auto-save (#1232)
- Hide block palette (#1319)
- Linebreaks in comments (#1338)
- Project screen reader support (#1332)
- Better forum quoter: Include BBCode (#1230)
- Cat blocks: Add blinking (#1310)
- Data category tweaks: Move reporters under operations section (#1300)
- Record project video: Support for sound recording (#1321)
- Record project video: Improve UI and add options (#1347)
- Show full areas: Support for signature settings (#1251)

#### Extension and Addon API

- `msg.locale` (#1314)
- `Trap.getBlockly` (#1331)
- JSDoc (#1339)

### Changed

#### Extension and Addon API

- Render tooltips above tags (#1318)
- Refactor traps (#1331)
- Show beta tag in settings popup (#1336)
- Show warnings in settings popup (#1336)
- Used incorrect cases README and CREDITS (#1344)
- Use SPDX indentifier in licenses (#1344)
- Add web worker support on userscripts (#1345)
- Bump intl-messageformat (#1348)
- Update localization strings

### Fixed

#### Addons

- Cat blocks: fix missing ears (#1306)
- Developer tools: Help window is incompatible with "Website dark mode" (#1372)
- Editor dark mode: Custom procedure modal title cut (#1372)
- Infinite scrolling: Remove blank space scratchr2 footer (#1375)
- More links: Addon blocks main thread (#1345)
- Scratch 2.0 → 3.0: Remix tree button color affected (#1275)
- Semicolon glitch: Semicolon has wrong color (#1297)
- Website dark mode: Emojis have white background (#1276)
- Website dark mode: Search bar made unreadable (#1360)
- Website dark mode: Message count made unreadable (#1365)

#### Extension and Addon API

- LocalizationProvider logs excessive amount of errors (#1335)
- Addons with permission requirements cannot be enabled on Firefox (#1359)

### Removed

#### Addons

- Fix "Load more" scrolling in search results (#1311)
- Highlight currently executing blocks: Remove notice (#1312)

#### Extension and Addon API

- Remove unused API Tab.getScratchVM (#1339)

## [v1.7.1] - 2021-01-11

### Fixed

#### Addons

- Website dark mode: Certain elements of the Scratch editor affected

## [v1.7.0] - 2021-01-10

### Added

#### Addons

- Better forum quoter (#1127)
- Cat blocks (#639)
- Data category tweaks (v2) (#1097)
- Mute project player (#1217)
- Semicolon glitch (#507)
- Scratch 2.0 → 3.0: Support for more pages (#1259)
- Sprite and script count: Block counter (#1121)
- Website dark mode: Support for more pages (#1259)
- Website dark mode: Support for post preview (#1160)
- Website dark mode: Support for syntax highlighting (#1160)

#### Extension and Addon API

- A way to disable popups (#1006)
- New popup for changing settings (#1006)
- A way to change Scratch colors (#1096)
- A way to set FPS to values other than 60 (#1131)
- A way to export and import settings (#1136)
- Support for easter egg addons (#1177)

### Changed

#### Extension and Addon API

- Messaging related addons no longer go to the top (#1242)
- Update localization strings

### Fixed

#### Addons

- Block switching: Addon does not work after switching languages (#1139)
- Block switching: Addon mishandles forever block (#1139)
- Cloud games: Add links to users (#1006)
- Colored context menus: No color when right-clicking the edge (#1119)
- Colored context menus: No color on new procedure arguments (#1119)
- Confirm actions: Addon runs on studios and topics (#1166)
- Developer tools: Optimize slow operations (#1120)
- Developer tools: Actions required multiple undos when reverting (#1120)
- Developer tools: CSS may cause encoding error (#1120)
- Developer tools: Extension blocks that are not orphaned can be removed (#1196)
- Hex color picker: Wrong background color on dark mode (#1142)
- Project notes tabs: Addon does not work in Firefox (#1117)
- Project notes tabs: Instructions do not fill empty space in Firefox (#1117)
- Project notes tabs: Errors when a section is missing (#1117)
- Project notes tabs: Projects with only instructions would have "Notes and Credits" on the tab (#1117)
- Project notes tabs: Buttons overlaps with remix credits (#1117)
- Project notes tabs: Addon loads on onload, rather than DOMContentLoaded (#1117)
- Project notes tabs: Description has a typo (#1190)
- Website dark mode: Studio thumbnail border does not affected (#1160)
- Website dark mode: Compatibility with other addons (#1160)
- Scratch 2.0 → 3.0: Color on usernames in Messages page affected (#1189)
- Scratch Messaging: Remove double escaping on tags (#1172)
- Scratch Notifier: Addon crashes when receiving crafted message (#1172)
- Scratch Notifier: Tags in project titles to emojis converted (#1172)

#### Extension and Addon API

- Update notification uses wrong font (#1125)
- Clicking outside "More Settings" modal does not close the modal (#1125)
- XSS filter does not escape quotes (#1128)
- Popup has two scrollbars (#1145)
- Extension option shows incorrect letters when localized (#1159)
- Uninstall URL still opens in prerelease (#1164)
- Popups are misaligned (#1187)
- Icons are blurry (#1243)
- getMsgCount errors when used in userscripts (#1245)
- Tooltips are misaligned (#1252)
- Site access screen opens on Firefox (#1258)

## [v1.6.1] - 2020-12-27

NOTE: All updates from [v1.6.0] are pushed on this version.

### Fixed

- Chrome enforces extensionName to be specified

## [v1.6.0] - 2020-12-27 [YANKED]

NOTE: v1.6.0 is only released on Firefox due to a special requirement by the Chrome Web Store related to localization. All updates are included on [v1.6.1].

### Added

#### Extension and Addon API

#### Addons

- Color picker (#1061)
- Record project video (#1083)
- Show my-ocular status: Support for profile pages (#1026)
- Studio manager tools: Add a way to leave studios from My Stuff (#1041)

### Changed

#### Extension and Addon API

- Update localization strings

### Fixed

#### Addons

- Thumbnails setter: Addon listed as a website addon (#1064)

#### Extension and Addon API

- Changing color settings may cause memory leak (#1062)

## [v1.5.1] - 2020-12-15

### Fixed

- Website dark mode: Comment loading screen is not dark (#1019)
- Onion skinning: Images got grouped unintentionally (#1037)

### Changed

#### Extension and Addon API

- Update localization strings

## [v1.5.0] - 2020-12-13

### Added

#### Addons

- Onion skinning (#879)
- Profile page banner (#895)
- Block switching: Support for more blocks (#979)
- Developer tools: Show broadcast senders and receivers (#980)
- Scratch 2.0 → 3.0: Support for /news (#941)
- Show full areas: Support for loading more in What's Happening (#899)
- Thumbnails setter: A way to disable thumbnail overwriting (#964)
- Website dark mode: Support for loading screen (#995)
- Website dark mode: Support for /news (#941)

#### Extension and Addon API

- Warning when posting on Japanese forum (#944)
- Warning when site access is off (#950)
- Button to open translation page (#1002)
- Notification for updates (#1016)
- "New" tag for addons (#1016)

### Changed

#### Extension and Addon API

- Load addons inside frames (#897)
- Update localization strings

### Fixed

#### Addons

- Customizable block colors: Addon did not affect devtools middle click feature (#669)
- Customizable block colors: Custom colors do not apply to custom blocks (#948)
- Customizable block colors: Custom colors do not apply to dropdowns (#956)
- Customizable block colors: Custom colors do not apply to extension blocks in non-English environment (#956)
- Customized quotes & code blocks on forums: Addon categorized as editor addon (#989)
- Mouse position: Addon crashes in project view (#954)
- Scratch Messaging: "Show More" button is partially hidden (#929)
- Scratch Messaging: Addon links to curators page for activity messages (#969)
- Scratch Messaging: Follower name links uses onClick (#969)
- Show my-ocular status: Addon is not localized (#925)
- Studio manager tools: Buttons don't have text when hovered (#994)
- Studio manager tools: Buttons don't have text when hovered (#994)
- Website dark mode: Project comments are unreadable with dark mode (#928)
- Website dark mode: Some pages are not listed in dark mode list (#949)
- Website dark mode: Addon still loads on editors (#960)
- Website dark mode: Addon does not make cloudmonitor rows dark (#960)
- Website dark mode: Addon changes variable monitor color (#981)
- Website dark mode: Addon styles in-editor Join Flow (#981)
- Website dark mode: Addon styles list row backgrounds when focused (#981)
- Website dark mode: Addon makes search input dark (#995)
- Website dark mode: Addon makes project warnings unreadable (#995)
- Some addons overflow in small stage (#930)
- Addons sometimes don't load in Firefox (#935)

#### Extension and Addon API

- Most translations don't load (#925)
- "Search" placeholder is not localized (#925)

## [v1.4.1] - 2020-12-03

### Fixed

#### Addons

- Forum search: Fix crashes (#901)
- Messages in editor: Typo in addon description (#903)
- Sprite and script count: Script count was inaccurate (#904)
- Addons have incorrect name (#887)

## [v1.4.0] - 2020-11-29

### Added

#### Addons

- Block switching (#768)
- Confirm actions (#797)
- Curator link (#725)
- Customized quotes & code blocks on forums (#694)
- Feature unshared projects (#757)
- Fix "Load more" scrolling in search results (#729)
- Fix broken SVG uploads (#748)
- Messages in editor (#607)
- Project notes tabs (#794)
- Show my-ocular status (#848)
- Sprite and script count (#732)
- Live featured project: Add option to disable alternative player (#707)
- Scratch Notifier: Studio activity url (#806)
- Website dark mode: Experimental Dark theme (#699)
- Website dark mode: Re-enable website dark mode (#699)
- Scratch 2.0 → 3.0: Support for more pages (#775)
- Scratch 2.0 → 3.0: Radius for change button on profile images (#832)
- Scratch 2.0 → 3.0: Smooth project borders (#851)

#### Extension and Addon API

- Localization (#753, #812, #823, #842, #867, #856, #854, #861)
- Support for %addon-self-dir% in themes CSS (#795)
- Setting warning and notice icons (#791)
- `key` property on manifest (#793)
- Source URL to theme CSS (#849)
- `CTRL + LEFT CLICK` addon name to show IDs instead of names (#874)

### Changed

#### Addons

- Display stage on left side: Add radius to backpack (#808)
- Forums image uploader: Clean up code (#829)
- Last edit tooltip: Show actual date instead of day (#734)
- Search profile: Add search profile username validator (#800)
- Show exact count: Faster, Better Forum User Count (#758)
- Forum search: Use better styling on the search bar (#668)

#### Extension and Addon API

- Make theme userstyles ordered (#704)
- Remove unnecessary word "theme" from the extension theme (#724)
- Update forum icon (#710)
- Make settings responsive (#828)
- Make licenses opening in new tab (#880)

### Fixed

#### Addons

- Clone counter: Fix negative clone count due to comparison error (#801)
- Developer tools: Fix white corners in predicate block when middle clicking (#781)
- Infinite scrolling: Fix fixed footer on annual report (#706)
- Infinite scrolling: Fix fixed footer showing behind projects (#735)
- Live featured project: Fix styling of forkphorus player (#707)
- More links: Fix addon not working properly by adding waitForElement for project pages (#433)
- Project notes tabs: Fix addon for remixes (#857)
- Project progress bar: Fix bug where progress bar broken on some languages (#711)
- Project progress bar: Fix some occasional style desyncs (#711)
- Project progress bar: Fix progress bar on updating assets (#711)
- Show exact count: Fix forum count showing just a number (#733)
- Show full areas: Fix capitalization on "Load more" (#722)
- Show full areas: Fix load more bug (#756)
- Thumbnails setter: Fix addon category to editor (#752)
- Website dark mode: Work around #701 (#699)
- Website dark mode: Fix minor CSS bug (#699)

#### Extension and Addon API

- Override checkbox style with custom style to fix Edge checkbox style (#787)
- Add missing favicon on the web pages (#723)
- Fix performance when dragging blocks in the editor (#747)
- Fix check for missing props (#870)
- Fix fallback for manifest l10n (#871)

### Removed

#### Addons

- Website dark mode: Remove Dark WWW theme (#876)

## [v1.3.3] - 2020-11-24

### Changed

#### Extension and Addon API

- Move libraries to the `libraries` folder (998781b)

## [v1.3.2] - 2020-11-24

### Fixed

#### Addons

- More links: Fix security issue due to faulty regular expression (GHSA-6qfq-px3r-xj4p, #827)

## [v1.3.1] - 2020-11-09

### Fixed

#### Addons

- Live featured project: Disable addon by default (#684)

## [v1.3.0] - 2020-11-08

### Added

#### Addons

- Live featured project (#633)
- Pause button (#619)
- Resizable comment input (#608)
- Thumbnails setter (#602)
- Last edit tooltip: Fix errors when the project is unshared (#629)
- Scratch Notifier: Add sound when you get a message (#595)
- Show full areas: Add load more button on profile page (#630)

#### Extension and Addon API

- More settings (#609)
- A warning on the Scratch forums to avoid posts about Scratch Addons (#626)
- Theme switch (#641)
- /* sa-autoupdate-theme-ignore */` (#652)

### Changed

#### Addons

- Dark mode editor: make fullscreen dark (#658)
- Editor dark mode: Style color picker on 3.Dark(er) (#656)
- Enable some old addons for all users on v1.3.0 (#655)
- Forums image uploader: Do not use project thumbnails (#653)
- Show full areas: Only load data if the user clicks "load more" (#665)

#### Extension and Addon API

- Revamp icons (#617)
- Remove dark mode default changer (#625)
- Revamp scrollbar design (#651)
- Many little UI changes & fixes (#659)
- Use `ESC` to clear search on settings page (#664)
- Add version name and open in new tab in the link to changelog in settings (#677)

### Fixed

#### Addons

- Better emojis: Remove extraneous bracket (#586)
- Better emojis: Add extraneous bracket back (#605)
- Customizable block colors: Add warning for traps (#629)
- Exact count: Fix on studios (#599)
- Infinite scrolling: Fix bug when showing your topics/posts in the forums (#601)
- Remix tree button on project pages: Fix remix button to work on all project pages (#581)
- Use dynamic CSS selector instead of static (#606)

#### Extension and Addon API

- Fix `.zip` download link (#577)
- Fix background console errors (#663)

### Removed

#### Extension and Addon API

- Remove prototype handler (#652)

## [v1.2.1] - 2020-10-27

NOTE: All updates from [v1.2.0] are pushed on this version.

### Fixed

#### Extension and Addon API

- Fix addon warning not showing (#571)

## [v1.2.0] - 2020-10-27 [YANKED]

NOTE: v1.2.0 is only released on Firefox due to an issue with perfomance warnings not showing. All updates are included on [v1.2.1].

***TODO***

## [v1.1.1] - 2020-10-11

NOTE: All updates from [v1.1.0] are pushed on this version.

### Fixed

#### Extension and Addon API

- Use webRequest instead of webNavigation (#457)

## [v1.1.0] - 2020-10-10 [YANKED]

NOTE: v1.1.0 is not released due to a permission issue. All updates are included on [v1.1.1].

### Added

#### Addons

- 60fps (#383)
- Better emojis (#402)
- Cloud games (#407)
- Display stage on left side (#376)
- Forum Search (#363)
- Scratch 2.0 → 3.0 (theme) (#359)
- Search profile (#405)

#### Extension and Addon API

- Access to addon settings via CSS variables (#439)
- Color input on settings (#400)
- General CSS around tabs in popup (#411)
- New links to credits and review pages (#414)
- Uninstall page (#437)
- Warnings, mainly to warn lags for addons that use addon.tab.traps (6a222c0)

### Changed

#### Addons

- Bitmap images copying: Add note to clear up confusion (#454)
- Cloud games: Add new scrollbar to cloud games (#412)
- Display stage on left side: Add warning
- Editor dark mode: Affect password input (#440)
- Editor dark mode: Change var(--text) to white on 3.Darker so that text is more readable
- Editor dark mode: Decrease font-weight from 800 to 700
- Editor dark mode: Don't inject dark mode into the remix tree (#420)
- Editor dark mode: Don't style scratch 3.0 search bar (#420)
- Editor dark mode: Remove a border that shouldn't be in 3.Dark and 3.Darker
- Image uploader: Slight updates (#371)
- Scratch Messaging: Make reply textbox more like Scratch (#375)
- Show full areas: Add expand button instead of all full signatures (#330)
- Show full areas: Clean signature expand button (#384)
- Show full areas: Cleaner expand signature
- Show full areas: Complete refactor of expand signature 
- Update tags and addon names (#422)

#### Extension and Addon API

- Ability to inject userstyles when the page starts loading (#328)
- Automatically update themes when changing settings (#252)
- Change end lines from CRLF to LF (#367)
- Change search to 150px (#378)
- Do not load traps unless addons that use them are enabled (#403)
- Hide settings page until it is loaded (0b3392c)
- Make better variable name (#446)
- Make sure the head loaded before injecting userstyles (#408)
- Run userscripts earlier, when the window load event triggers (#429)

### Removed

#### Extension and Addon API

- "Changed by [line of code]" console logs (#419)

### Fixed

#### Addons

- Scratch Messaging: Fix link to studio comments (#356)
- Scratch Messaging: Ignore Set-Cookie inside comment endpoint (#331)
- Scratch Notifier: Fix studio comments don't notify with the full comment content

#### Extension and Addon API

- Fix Vue warns (#355)
- Fix bug in URL/pattern matcher when addon runs if manifest has no trailing slash (#332)
- Fix messageForAllTabs() not working properly in Firefox (#386)
- Fix modifying "select" setting not disabled if addon disabled (#353)

## [v1.0.0] - 2020-09-24

Initial release.

[v1.16.3]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.16.3
[v1.16.2]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.16.2
[v1.16.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.16.1
[v1.16.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.16.0
[v1.15.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.15.0
[v1.15.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.15.0
[v1.14.3]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.14.3
[v1.14.2]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.14.2
[v1.14.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.14.1
[v1.14.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.14.0
[v1.13.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.13.0
[v1.12.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.12.1
[v1.12.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.12.0
[v1.11.2]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.11.2
[v1.11.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.11.1
[v1.11.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.11.0
[v1.10.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.10.0
[v1.9.3]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.9.3
[v1.9.2]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.9.2
[v1.9.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.9.1
[v1.9.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.9.0
[v1.8.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.8.1
[v1.8.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.8.0
[v1.7.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.7.1
[v1.7.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.7.0
[v1.6.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.6.1
[v1.6.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.6.0
[v1.5.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.5.1
[v1.5.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.5.0
[v1.4.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.4.1
[v1.4.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.4.0
[v1.3.3]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.3.3
[v1.3.2]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.3.2
[v1.3.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.3.1
[v1.3.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.3.0
[v1.2.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.2.1
[v1.2.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.2.0
[v1.1.1]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.1.1
[v1.1.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.1.0
[v1.0.0]: https://github.com/ScratchAddons/ScratchAddons/releases/tag/v1.0.0

<!--

# Heading format

Here's the simple format. Other types such as "Removed" can be added later.

### Added

#### Addons

#### Extension and Addon API

### Changed

#### Addons

#### Extension and Addon API

### Fixed

#### Addons

#### Extension and Addon API

# RegEx for @apple502j's changelog

Find      : `    (#\d+) (.+)\. \(prio-\d\)`
Replace   : `- $2 \($1\)`

-->