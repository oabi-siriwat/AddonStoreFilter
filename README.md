# Add-on store Filter

- Author: Oabi Siriwat
- NVDA compatibility: 2024.1 and later (last tested with 2026.3)
- Download: https://github.com/oabi-siriwat/AddonStoreFilter/releases/latest/download/AddonStoreFilter.nvda-addon

Add-on store Filter makes the NVDA Add-on Store quicker to use. Press one key to hear one detail of the selected add-on, without opening the Other Details box. You can also choose which details NVDA speaks while you move through the add-on list, and in which order.

## Commands in the Add-on Store

These keys work while the Add-on Store window is open and active. In other windows they do nothing.

- **NVDA+Control+1:** Status. Example: Status. Enabled
- **NVDA+Control+2:** Version. On the Installed tabs it is the installed version, on the Available tab the available version. Example: Installed version. 26.11.2
- **NVDA+Control+3:** Channel. Example: Channel. Stable
- **NVDA+Control+4:** Author. For an add-on that is not installed, the store only knows the publisher, so you hear Publisher instead.
- **NVDA+Control+5:** Publication date. Example: Publication date. 11/12/2026
- **NVDA+Control+6:** Install date. Example: Install date. 11/13/2026
- **NVDA+Control+7:** Minimum NVDA version. Example: Minimum NVDA version. 2026.3
- **NVDA+Control+8:** Last tested NVDA version. Example: Last tested NVDA version. 2026.3.1

If the add-on has no value for a detail, you hear "none". Dates use your Windows date format.

## Choosing what the add-on list reads

Go to **NVDA Menu, Preferences, Settings, Add-on store Filter**.

- **Details read in the add-on list:** while you move through the list with the arrow keys, NVDA always reads the add-on name first, then the details you tick here, in the order of the list. Use Move Up and Move Down to change the order. Nothing is ticked at first, so you hear only the add-on name. With everything ticked, you hear all the details, like NVDA without this add-on.
- **Select All / Deselect All:** ticks or unticks every item.
- **Reset to default:** puts the items back in the first order, unticked.
- **Check for update:** looks for a newer version now.

Details that the selected add-on does not have are skipped.

## Changing the keys

Go to **NVDA Menu, Preferences, Input gestures**, and open the **Add-on store Filter** category. The commands are listed in key order, from "1 status of the selected add-on" to "8 last tested NVDA version of the selected add-on".

## Updates

When NVDA starts, the add-on quietly checks GitHub for a newer version. If there is one, it asks whether to download and install it. You can also press Check for update in the settings.

## Changelog

### v1.0

- First release.
