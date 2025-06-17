# Staff Commands

## List of commands for all staff

---

### Commands for Mods and higher

- /gamemode 

  - (Required) `creative`, `survival`, or `spectator`

  - If you are spectating someone, use `/spectate <username>`

- [/invsee &lt;username&gt;](https://www.spigotmc.org/resources/inventory-rollback-plus-1-8-1-21-5.85811/#:~:text=Documentation-,Commands,-/irp%20restore%20%5Bname)

  - Shows a GUI, of the persons current inventory & armour slots.

  - You can drag items out of the GUI and the item will be taken out or moved around the persons inventory/armour slots if needed.

- [/irp restore &lt;username&gt;](https://www.spigotmc.org/resources/inventory-rollback-plus-1-8-1-21-5.85811/#:~:text=Documentation-,Commands,-/irp%20restore%20%5Bname)

  - Shows a GUI, of every time their full inventory was backed up and saved automatically.

  - Clicking on the chest will open another GUI showing their full inventory at that time, you can then click the nether star to override their inventory with that backup.

  - More information can be found [here about this plugin](https://www.spigotmc.org/resources/inventory-rollback-plus-1-8-1-21-5.85811/).

- [/co restore](https://docs.coreprotect.net/commands/#co-restore)

  - (Required) Specifying `radius:<radius>` (e.g `20` for 20 blocks around you or `#global` for the whole server.)

  - (Required) Specifying `time:<time>` (e.g `1h` for 1 hour or `10m` for 10 minutes, to restore the specified radius the amount of time specified. - This should be a time before the roll back occurred)

  - (Recommended) Specifying `user:<username>` to only restore this persons actions prior to them being rolled back.

WorldEdit and Spawn Building Privileges can be requested from an Op

---

### All staff have access to the follow commands

[**CoreProtect plugin**](https://docs.coreprotect.net/commands/)**:**

- [/co inspect](https://docs.coreprotect.net/commands/#co-inspect)

  - Enabled and disabled by running the same command again.

  - Used for when you want to find out who broke, placed a block or added/removed items from a chest.

- [/co rollback](https://docs.coreprotect.net/commands/#co-rollback)

  - (Required) Specifying `radius:<radius>` (e.g `20` for 20 blocks around you or `#global` for the whole server.)

  - (Required) Specifying `time:<time>` (e.g `1h` for 1 hour or `10m` for 10 minutes, to roll back the specified radius the amount of time specified.)

  - (Recommended) Specifying `user:<username>` to only roll back this persons actions.

- [/co lookup](https://docs.coreprotect.net/commands/#co-lookup)

  - Similar to `/co inspect` as in, it tells you who performed what actions and where. This command allows you to check across the whole server for actions performed.

  - If multiple pages are returned, use the command `/co lookup <page number>` to look at that page.

  - (Optional) Specifying `radius:<radius>` (e.g `20` for 20 blocks around you or `#global` for the whole server.)

  - (Required) Specifying `time:<time>` (e.g `1h` for 1 hour or `10m` for 10 minutes, to look back the amount of time specified.)

  - (Recommended) Specifying `user:<username>` to only look back on this persons actions.

  - (Optional) Specifying `action:<action>` (e.g `+block` for blocks placed, `-block` for blocks broken, `block` for blocks placed & broken, `chat` for chat messages sent, `+container` for items put in chests, `-container` for items removed from chests, `container` for items put in or removed from chests, `+inventory` for items added to their inventory, `-inventory` for items removed from their inventory, `inventory` for items added or removed from their inventory, `+item` for items picked up, `-item` for items dropped, `item` for items picked up or dropped) See all actions [here on docs.coreprotect.net](https://docs.coreprotect.net/commands/#aaction)

  - (Optional) Specifying `include:<include>` to only look for a specific block or entity.

  - (Optional) Specifying `exclude:<exclude>` to exclude a block or entity from the look up.

**Punishments plugin:**

- /ban &lt;username&gt; \[reason\]

  - This will disconnect someone and prevent their access to the server permanently, someone can always be unbanned at a later date or the ban length be adjusted. Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason., someone can always be unbanned at a later date or the ban length be adjusted. Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason.

- /tempban &lt;username&gt; &lt;length&gt; \[reason\]

  - This will disconnect someone and prevent their access to the server for the specified length (e.g `3h` for 3 hours or `7d` for 7 days), someone can always be unbanned at a later date or the ban length adjusted. Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason.

- /kick &lt;username&gt; \[reason\]

  - This will disconnect someone from the server. Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason.

- /mute &lt;username&gt; \[reason\]

  - This will prevent someone from sending chat messages or DMing others in-game permanently. Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason.

- /tempmute &lt;username&gt; &lt;length&gt; \[reason\]

  - This will prevent someone from sending chat messages or DMing others in-game for the specified length (e.g `3h` for 3 hours or `7d` for 7 days). Reason is optional, but highly recommended to make it easier in the future for staff to look back on why someone was punished.

  - If a rule was broken, use `/punish`. If something isn't specified in the punish GUI, please specify a detailed reason.

- /history \[username\]

  - Shows a GUI of the most recent punishments.

  - (Optional) Specifying `username` will show that persons most recent punishments.

- /punish &lt;username&gt;

  - Shows a GUI, with predefined reasons & lengths. That align with the servers rules & punishment guidelines.

  - It remembers how many punishments have occurred previously, so a higher level of punishment can be handed out in future. 

  - Hover over the glass panes to show specific punishments, clicking on them will hand out that punishment to the specified person.

  - At the moment, it is not recommended to rollback a permanently banned person, in case they submit an appeal. It is suggested you wait a week to see if they submit an appeal or their ban length is adjusted, if they do not you should rollback their actions 60 days using CoreProtect.

- /spectate or /spec &lt;username&gt;

  - Spectate the specified person from their point of view.

- /spectate stop or /spec stop

  - Stops spectating the person, puts you back into survival and teleports you to spawn.

- /tp &lt;username&gt;

  - Teleport yourself to the specified person, without needing to request. It does not tell the person that you have teleported.

- /tphere &lt;username&gt;

  - Teleports the specified person to yourself, without needing to request. It does not tell the person that they have been teleported.

- /tppos &lt;x&gt; &lt;y&gt; &lt;z&gt;

  - Teleport yourself to specified coords, in the current world. You can replace any of the coords with `~` to use your current location.

- /chat staff or /staff 

  - Switches your in-game chat to a staff only visible chat. It remains like this until you switch back to global chat. (Even if you log off and log back in.)

  - Messages you type in chat will be sent to this staff only chat.

  - If you prefer to stay in global chat, but be able to send a message to staff only chat without needing to switch. Use `/staff <message>`

- /chat global or /global 

  - Switches your in-game chat to a global chat, visible to everyone. It remains like this until you switch to another chat. (Even if you log off and log back in.)

  - Messages you type in chat will be sent to this chat.

  - If you prefer to stay in staff chat, but be able to send a message to global chat without needing to switch. Use `/global <message>`
