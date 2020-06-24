# ChangeLog
## 0.2.9
### :stars: Improvements
- updated interface again :)


## 0.2.8
### :stars: Improvements
- Updated notes panel so its more compact.
- You can now favorite a document by clicking on the star at the top of the documents title.
- Added a search filter to only show documents that contain the search query.


## 0.2.7
### :wrench: Fixes
- potential fix for freezing after the app has been idle for a while (thanks @rachid!)

## 0.2.6
### :tada: New
- you can now publish your notes, they will be available (for now) at `https://devnotes.beta.af/<username>`

## 0.2.5
### :tada: New
- Added a warning indicator when we detect that we are offline.

### :wrench: Fixes
- 100% CPU usages and unresponsiveness if the editor had a document open, went offline and came online again.

## 0.2.4

### :tada: New
- Cmd-A now selects all even when in Vim Normal mode.
- Autocomplete for emojis: If you start typing `:c` it will popup an autocomplete list with matching emojis. Press enter to insert it.

### :wrench: Fixes
- CPU usage: As we increased the login token validity to 31 days, we broke the 32bit limit in milliseconds that was used for the setInterval to refresh the token, effectively causing it to try and refresh the token every millisecond. we no clamp the value to a minimum of once per minute and a maximum of once per hour.
- The markup button for Bold now actually makes something bold instead of italic :)

## 0.2.3

### :wrench: Fixes

The markup button for Bold now actually makes something bold instead of italic :)
z-index issue regarding the split lines


## 0.2.2

### :tada: New
- You can now restore notes to a previous state.

### :stars: Improvements
- Toolbar items now stack
- Updated history panel

## 0.2.1

### :wrench: Fixes
- disabled version saves as this caused a bug

## 0.2.0

### The second premium feature, Collaborative Editing, is here !
You can now create teams, invite members, and share your notes with them.
Everyone can edit the note simultaneously and you will see their cursors and changes in realtime.
If collaborators are connected, they will show up in the bottom bar indicating which color caret belongs to which user.

### :tada: New
- Create teams
- Invite members
- Share notes
- Collaborative Editing
- Versioning : Every document save will create a new version. This will allow us in the future to view or rollback to previous versions.

## 0.1.9

### :wrench: Fixes
- windows build

## 0.1.8

### Support for admonitions
You can now create admonitions by using the following syntax:
```
:::tip A tippy tip
This is pretty great!
:::
```

Which will display like.

:::tip A tippy tip
This is pretty great!
:::

Do note you can still embed code inside the admonitions :)

Here are a few variants:

:::note Just a simple note
A simple important message
:::

:::important An important message
A simple important message
:::

:::caution This is dangerous
A simple important message
:::

:::warning This is a Warning
A simple important message
:::

The toolbar also contains new entries to create these admonitions.

### :stars: Improvements

Added a table icon that inserts an example table if nothing is selected.

## 0.1.7

### The first premium feature, Grammar Checking, is here !
The first button in the new toolbar triggers a grammar check. You will see a small progress indicator as soon as you click it. Wait for the progress to be done and you will see red underlines on words that are grammatically incorrect or misspelled.

Hover over those lines and you get a bunch of suggestions. You will also be able to add words to your local or global dictionary, or, Ignore rules for this note or all your notes.

### A shiny new Toolbar :tada:

The code editor now has a toolbar to help you with formatting the text.
You can click the select some text and click the buttons to apply the formatting.

You can also use the following keyboard shortcuts:

- `Cmd-B` bold
- `Cmd-I` italic
- `Cmd-1` h1
- `Cmd-2` h2
- `Cmd-3` h3
- `Cmd-4` h4
- `Cmd-5` h5
- `Cmd-6` h6
- `Cmd-.` quote'
- `Cmd-X` toggleCheckBox

For our windows users, replace Cmd with Ctrl.

### Table support
We\`ve made it easier to create tables. Just start on a new line with a pipe `|` and type a header. Then press `tab` to get the next column or enter to procesed to the next row.
If you are done with the table just press `CMD-Enter` or `CTRL-Enter` and you can continue as usual.

The following keyboard shortcuts are available while editing a table:

  - `Tab` Next column
  - `Shift-Tab` Previous Column
  - `Enter` Newt Row
  - `Cmd-Enter` End Table
  - `Shift-Cmd-Left` Align column to the left
  - `Shift-Cmd-Right` Align column to the right
  - `Shift-Cmd-Up` Move row up
  - `Shift-Cmd-Down` Move row down
  - `Cmd-Left` Next Cell
  - `Cmd-Right` Previous Cell
  - `Cmd-Up` Cell Above
  - `Cmd-Down` Cell Below

This is an example of how to create a table:

```
| First Name | Last Name | Email               |
| ---------- | --------- | ------------------- |
| John       | Smith     | J.Smith@example.com |
| Jane       | Doe       | J.Doe@example.com   |
```


### :stars: Improvements
- Code blocks that do not specify a language will no longer show line numbers
- Code blocks that are smaller than or equal to 10 lines will no longer show line numbers
- These changes will be configurable in the future

### :wrench: Fixes
- Auto-tagger should now behave again.

## 0.1.6
### :tada: New
- Sync scroll views from editor to viewer :arrow_up_down:

### :stars: Improvements
- Viewer now renders like a blog post :sunglasses:
- Safari should now render correctly as well :tada:
- Electron windows have custom scrollbars :fireworks:

### :wrench: Fixes
- Multiple Mermaid render fix thanks to @rachid :tropical_fish:

## 0.1.5
- Updated the viewer style with better contrasting colors, font spacing and several other improvements

## 0.1.4
- Added feedback button
- Updated updater window

## 0.1.3
- Created first windows installer release

## 0.1.2
- Added auto update support
- Created first MacOS DMG release

## 0.1.1
- added embedly plugin
- added auto tag plugin

## 0.1.0
- initial release
