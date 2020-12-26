# Take Notes

## Divinity: Original Sin 2 - Definitive Edition

----------

Editable notebooks! Take _notes_, keep a record of _events_ and _characters_, and write about your _deeds_ (or _misdeeds_) as you adventure through Rivellon. Author the most comprehensive compendium of knowledge that transcends even Cranley Huwbert's! or just make a todo-list. _Create_, _View_, _Edit_ your entries in-game or externally.

## Releases

* ~~***[Steam Workshop]()***~~
* ***[Github](https://github.com/Shresht7/Take-Notes)***
* ~~***[Nexus]()***~~

## Requirements

* ***[Script-Extender](https://github.com/Norbyte/ositools)***
* ***[UI Components Library](https://github.com/Shresht7/UI-Components-Library)***

## Features

* Maintain your own personal **Journal**.
* The mod adds **editable notebooks** to **Story** and **GM modes**.
* _Notebooks_ have been integrated into vanilla _treasure-tables_. They will appear as **loot** and you can buy them from traders.
* _Notebooks_ can also be **crafted**. `LeatherScraps + Needle-&-Thread + 3x Sheet-of-Paper`
* _Create_, _View_, and _Edit_ your entries from an in-game UI.
* Notebook contents can be saved on a _per-character_ or _per-item basis_.

![Journal](https://imgur.com/tHcOoGF.png)

>NOTE: The notebook contents are _saved_ when the UI is closed. So make sure to close it when you're done. This is especially important to keep in mind if you use multiple notebooks. Opening a different notebook when the UI is open will cause the contents to get mixed-up. Just close the first one before you open the next.

## ModSettings

Players can change mod-settings by editing the global settings file (`S7Central.json`) in the `Osiris Data` folder. (`..\Documents\Larian Studios\Divinity Original Sin 2 Definitive Edition\Osiris Data\S7Central.json`). The internal identifier for the mod is `S7_Journal`.

### Uniques

The `Uniques` option is for people who want access to these notebooks from the very beginning. However only one will spawn per player character.

* if **`Uniques`** is set to true, each player will be granted one unique notebook when the game starts. They will not spawn as loot or treasure however. (Default: `false`)

### Storage

Storage mode dictates how the contents of the notebooks are saved.

* **`Internal`** storage mode saves the contents of the notebooks in the save-file itself. Notebook contents will be a part of your save. (Default)
* **`External`** storage mode saves the contents of the notebooks in an external json file in `Osiris Data`. This allows you to edit them outside the game. 

### SyncTo

Notebook contents can be saved on a per-character or per-item basis.

* **`CharacterGUID`**: If saved on a per-character basis, each character will have a unique notebook. Opening any notebook item will always open the one associated to them.
* **`ItemGUID`**: When synced on a per-item basis, each notebook will hold its own content. (Default)

## Console-Commands

The following console-commands are available for the player to use. The general format for the commands is `!S7_Journal <Command> <Arguments>`.

| command                                  | result                                                                        |
| ---------------------------------------- | ----------------------------------------------------------------------------- |
| `AddJournal`                             | A new notebook will be added to the host character's inventory                |
| `ResyncSettings`                         | Reloads and reapplies mod-settings from the `S7Central.json` file             |
| `ListPersistentJournals`                 | Prints a list of saved entries in PersistentVars                              |
| `ExportPersistentJournals <JournalName>` | Export entry from PersistentVars to OsirisData. Use `all` to export all       |
| `ImportFromOsirisData <JournalName>`     | Import entry from OsirisData.                                                 |
| `RemoveJournal <JournalName>`            | Removes the entry from PersistentVars. Use `all` to clear persistent-vars out |

>Note: Console-Commands need the script-extender's **debug-console** which can be enabled by setting `DeveloperMode` and `CreateConsole` to true in `OsirisExtenderSettings.json`.

----------

## Thanks and Credits

* [**Divinity: Original Sin 2**](http://store.steampowered.com/app/435150/Divinity_Original_Sin_2/), a game by **[Larian Studios](http://larian.com/)**.
* **LaughingLeader** for the **[Source Control Generator](https://github.com/LaughingLeader/SourceControlGenerator)**.
* **Norbyte** for The **[Script-Extender](https://github.com/Norbyte/ositools)**.
* **Sebastian Lenz** and **LaughingLeader** for the **[VSCode extension](https://marketplace.visualstudio.com/items?itemName=sebastian-lenz.divinity-vscode)**.




