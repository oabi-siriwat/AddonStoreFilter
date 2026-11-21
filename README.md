# Add-on store Filter

- Author: Oabi Siriwat
- NVDA compatibility: 2024.1 and later (last tested with 2026.3)
- Download: https://github.com/oabi-siriwat/AddonStoreFilter/releases/latest/download/AddonStoreFilter.nvda-addon

Add-on store Filter makes the NVDA Add-on Store quicker to use. Press one key to hear one detail of the selected add-on, without opening the Other Details box. You can also choose which details NVDA speaks while you move through the add-on list, and in which order.

## Commands in the Add-on Store

These keys work while the Add-on Store window is open and active. In other windows they do nothing.

- **NVDA+Control+1:** Name. Example: Name. Clip Contents Designer
- **NVDA+Control+2:** Description: what the add-on does.
- **NVDA+Control+3:** Status. Example: Status. Enabled
- **NVDA+Control+4:** Version. On the Installed tabs it is the installed version, on the Available tab the available version. On the Updatable tab you hear both, so you know which version you will get. Example: Installed version. 1.0, Available version. 1.1
- **NVDA+Control+5:** Channel. Example: Channel. Stable
- **NVDA+Control+6:** Author. For an add-on that is not installed, the store only knows the publisher, so you hear Publisher instead.
- **NVDA+Control+7:** Publication date. Example: Publication date. 11/12/2026
- **NVDA+Control+8:** Install date. Example: Install date. 11/13/2026
- **NVDA+Control+9:** Minimum NVDA version. Example: Minimum NVDA version. 2026.3
- **NVDA+Control+0:** Last tested NVDA version. Example: Last tested NVDA version. 2026.3.1

If the add-on has no value for a detail, you hear "none". Dates use your Windows date format.

## Choosing what the add-on list reads

Go to **NVDA Menu, Preferences, Settings, Add-on store Filter**.

- **Details read in the add-on list:** while you move through the list with the arrow keys, NVDA always reads the add-on name first, then the details you tick here, in the order of the list. The list has the details of NVDA+Control+3 to 0; name and description are only read with their keys. Use Move Up and Move Down to change the order. Nothing is ticked at first, so you hear only the add-on name. With everything ticked, you hear all the details, like NVDA without this add-on.
- **Select All / Deselect All:** ticks or unticks every item.
- **Reset to default:** puts the items back in the first order, unticked.
- **Check for update:** looks for a newer version now.

Details that the selected add-on does not have are skipped.

## Changing the keys

Go to **NVDA Menu, Preferences, Input gestures**, and open the **Add-on store Filter** category. The commands are listed in key order, from "01 name of the selected add-on" (NVDA+Control+1) to "10 last tested NVDA version of the selected add-on" (NVDA+Control+0).

## Updates

When NVDA starts, the add-on quietly checks GitHub for a newer version. If there is one, it asks whether to download and install it. You can also press Check for update in the settings.

## Changelog

### v1.1

- New keys: NVDA+Control+1 reads the name, NVDA+Control+2 the description. The other details moved to NVDA+Control+3 to 0.
- On the Updatable tab, the version key reads both the installed and the available version.

### v1.0

- First release.
