# Add-on store Filter

- Author: Oabi Siriwat
- NVDA compatibility: 2024.1 and later (last tested with 2026.3)
- Download: https://github.com/oabi-siriwat/AddonStoreFilter/releases/latest/download/AddonStoreFilter.nvda-addon

Add-on store Filter makes the NVDA Add-on Store quicker to use. Press one key in the add-on list to hear one detail of the selected add-on, without going to the Other Details box. You can also choose which details NVDA speaks while you move through the add-on list, and in which order.

## Commands in the Add-on Store

These keys work in the add-on list of the Add-on Store: the number keys above the letters, and the minus key next to 0. In the search field and the other controls they type as usual, and in other windows they do nothing.

- **1:** Name. Example: Name. Clip Contents Designer
- **2:** Description: what the add-on does.
- **3:** Status. Example: Status. Enabled
- **4:** Version. On the Installed tabs it is the installed version, on the Available tab the available version. On the Updatable tab you hear both, so you know which version you will get. Example: Installed version. 1.0, Available version. 1.1
- **5:** Channel. Example: Channel. Stable
- **6:** Author. For an add-on that is not installed, the store only knows the publisher, so you hear Publisher instead.
- **7:** Publication date. Example: Publication date. 11/12/2026
- **8:** Install date. Example: Install date. 11/13/2026
- **9:** Minimum NVDA version. Example: Minimum NVDA version. 2026.3
- **0:** Last tested NVDA version. Example: Last tested NVDA version. 2026.3.1
- **- (minus):** Other Details: everything in the store's Other Details box, such as publisher, ID, links, license and VirusTotal results. It also works when that box is hidden. The minus key works with any keyboard layout, for example Thai.

If the add-on has no value for a detail, you hear "none". Dates use your Windows date format.

## Switching tabs from the add-on list

In the add-on list, press **Right Arrow** for the next tab and **Left Arrow** for the previous one. You stay in the list, so you do not have to press Tab to get back to it. NVDA says the tab name, then how many add-ons it has once its list has loaded, then the selected add-on. On the last tab, Right Arrow says "Already at the last tab"; on the first tab, Left Arrow says "Already at the first tab". To go round from the last tab to the first instead, check **Wrap around tabs** in the context menu or in the settings.

The add-on remembers where you were in each tab while the store is open. When you come back to a tab, the same add-on is selected again. A tab you have not visited yet starts at its first add-on. When you close the store, this is forgotten.

Like changing tabs the normal way, switching tabs clears the search field.

## The add-on list's context menu

In the add-on list, open the context menu (Applications key or Shift+F10, or Enter on an add-on). Below the store's own actions for the add-on are seven items, one for each box in the store window.

These five are submenus. Each one starts with **Show in the store window**, followed by the box's own choices:

- **Sort by column:** the sort choices, for example Name (ascending), Name (descending), Status (ascending). The current one is checked.
- **Channel:** All, Stable, Beta, Dev, and External on the Installed tabs.
- **Enabled/disabled:** All, Enabled, Disabled. It filters the installed add-ons, so the store has this box only on the Installed tabs. On the Available and Updatable tabs the submenu has Show in the store window and the line "(Only on the Installed tabs)", which cannot be chosen.
- **Include incompatible add-ons:** a check item to also list store add-ons that are not compatible with your NVDA but can still be installed. This is not the Installed incompatible add-ons tab, which lists incompatible add-ons already installed. The store has this box only on the Available and Updatable tabs; on the Installed tabs the submenu has Show in the store window and the line "(Only on the Available and Updatable tabs)".
- **Search:** **Search for...** opens a box to type your search (leave it empty to show all add-ons). **Clear search** appears when a search is active.

The choices work even while the box is hidden, so you can hide a box and still change it from the menu. Choosing one changes the store's own box, so the result is the same as changing it by hand.

These two are plain check items, because they have no choices:

- **Description:** the description box in the details on the right.
- **Other Details:** the box below it with the publisher, ID, links, license and the other details.

For every box, checked means it is shown in the store window, as usual. Uncheck it, and the box disappears, so Tab skips it. Check it again to bring the box back. NVDA says, for example, "Search hidden" or "Search shown", and the focus goes back to the list. All seven are shown at first.

After a separator comes **Wrap around tabs**. Unchecked (the default), Left and Right Arrow stop at the first and last tab. Checked, they go round from the last tab to the first and back.

The add-on remembers your choices, also after closing the store or restarting NVDA. The same settings are in the Context menu group of the settings. Hiding Search also empties it, so no hidden search keeps filtering the list. As before, Enabled/disabled only appears on the Installed tabs, and Include incompatible add-ons only on the Available and Updatable tabs; checking them does not add them to the other tabs. Hiding Include incompatible add-ons keeps its current setting. With Description or Other Details hidden, the keys still read those details (2 for the description, minus for Other Details).

When no add-on is selected, for example in an empty list, the context menu shows these items alone, so you can always bring a box back.

## Settings

Go to **NVDA Menu, Preferences, Settings, Add-on store Filter**. The settings are in three groups.

### Add-on list

- **Details read in the add-on list:** while you move through the list with the arrow keys, NVDA always reads the add-on name first, then the details you tick here, in the order of the list. The list has the details of keys 3 to 0; name, description and Other Details are only read with their keys. Use Move Up and Move Down to change the order. Nothing is ticked at first, so you hear only the add-on name. With everything ticked, you hear all the details, like NVDA without this add-on.
- **Select All / Deselect All:** ticks or unticks every item.
- **Reset to default:** puts the items back in the first order, unticked.

Details that the selected add-on does not have are skipped.

### Tabs

- **Tabs shown in the Add-on Store:** the store's tabs in the order they appear. Uncheck a tab to hide it. Use Move tab up and Move tab down to change the order. At least one tab must stay checked. The change takes effect the next time you open the Add-on Store. If NVDA wants to open the store on a hidden tab, it opens on a shown one instead.
- **Reset tabs:** puts the tabs back in NVDA's order, all shown.

### Context menu

**Context menu items:** one list with the same items as the add-on list's context menu, in the same order: Sort by column, Channel, Enabled/disabled, Include incompatible add-ons, Search, Description, Other Details, and last Wrap around tabs. For the boxes, checked = shown; if the store is open, it changes as soon as you press OK or Apply. Wrap around tabs is unchecked by default.

### Other

- The move buttons in both lists say the new position, for example "Version, 2 of 8". On the first item, Move Up says "Already at the top"; on the last item, Move Down says "Already at the bottom".
- **Check for update** (below the groups): looks for a newer version now.

## Changing the keys

Go to **NVDA Menu, Preferences, Input gestures**, and open the **Add-on store Filter** category. The detail commands are named after the detail, for example "Name of the selected add-on" (1), "Author of the selected add-on" (6) and "Other details of the selected add-on" (minus), and listed in alphabetical order. The category also has "Next Add-on Store tab" (Right Arrow) and "Previous Add-on Store tab" (Left Arrow).

## Updates

When NVDA starts, the add-on quietly checks GitHub for a newer version. If there is one, it asks whether to download and install it. You can also press Check for update in the settings.

## Changelog

### v1.5

- On tabs where the store has no Enabled/disabled or Include incompatible add-ons box, their submenu now says where the box is: "(Only on the Installed tabs)" or "(Only on the Available and Updatable tabs)".

### v1.4

- In the add-on list's context menu, Sort by column, Channel, Enabled/disabled, Include incompatible add-ons and Search are now submenus. Each has "Show in the store window" and the box's own choices, for example Name (ascending) or Stable, so you can sort, filter and search from the menu, even with the box hidden.

### v1.3

- The details are now read with the keys 1 to 0 alone in the add-on list, instead of NVDA+Control+1 to 0. In the search field these keys type as usual.
- New key: minus (next to 0) reads the store's Other Details box, on any keyboard layout.
- In Input gestures, the commands are named after the detail without a number in front, for example "Author of the selected add-on".
- Left and Right Arrow in the add-on list switch tabs without leaving the list. NVDA says the tab and its number of add-ons, and remembers the selected add-on in each tab. They stop at the first and last tab unless Wrap around tabs is checked.
- New setting: reorder the Add-on Store tabs or hide the ones you do not use.
- The add-on list's context menu has check items to show or hide the Sort by column, Channel, Enabled/disabled, Include incompatible add-ons, Search, Description and Other Details boxes of the store, and to turn Wrap around tabs on or off.
- The settings are now in three groups: Add-on list, Tabs and Context menu. The Context menu group has one list with the same items as the menu.
- The Move Up/Down buttons in the settings say the new position, or that the item is already at the top or bottom.

### v1.1

- New keys: NVDA+Control+1 reads the name, NVDA+Control+2 the description. The other details moved to NVDA+Control+3 to 0.
- On the Updatable tab, the version key reads both the installed and the available version.

### v1.0

- First release.
