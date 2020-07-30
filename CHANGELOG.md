### 0.2.8
- **Fix**: Fixed bug were variables inside built-in events available in all scopes
- **Fix**: Fixed bug were built-in events were allowed multiple times
- **New**: Added initial support for "live coding" by setting the scene script in the currently open scene directly while OffAir (<kbd>ctrl</kbd>-<kbd>shift</kbd>-<kbd>F5</kbd>)
- **Change**: Removed "OnAir check" for (<kbd>ctrl</kbd>-<kbd>F5</kbd>) to be able to validate code without being OnAir
- **Change**: Option `vizscript.compiler.hostPort` - Default port changed to 6998 to be able to work OffAir

---

### 0.2.7
- **Fix**: Fixed another bug that could sometimes result in the extension crashing

---

### 0.2.6
- **Fix**: Fixed bug were reopening VS Code would sometimes result in the extension crashing

---

### 0.2.5
- **Fix**: Resolved small issue with snippet completions. Global Procedures without parameters or with overloads will no longer use snippet completions

---

### 0.2.4
- **New**: Initial support for snippet completions on Global Procedures. This feature will autofill placeholder values in the parameters and <kbd>tab</kbd> will jump to the next parameter.(disabled by default)
- **New**: Option `vizscript.enableGlobalProcedureSnippets` - Enable snippet completions for Global Procedures
!["Snippet completions"](images/snippet_completions.png)

---

### 0.2.3
- **New**: Support for both Scene and Container scripts
- **New**: The extension now contributes two languages `VizSceneScript` and `VizContainerScript`
- **New**: "This" keyword enables context sensitive completions based on the language selected
- **New**: Script type will automatically be selected when a file is opened based on the file extension
  - Scene scripts: `.vs .viz .v3script `
  - Container scripts: `.vsc .vizc`

---

### 0.2.2
- **New**: Added documentation support for document completions. Functions, subs and variables supported for now.
	- A comment directly above a function or sub will be used as description.
  	
		!["Function description"](images/function_description.png)
  - A comment directly after a variable declaration will be used as description.
    
    !["Variable description"](images/variable_description.png)

---

### 0.2.1
- **Fix**: Rewrote line logic to support nested brackets and parantheses
- **Change**: Improved support for Arrays

---

### 0.2.0
- **Change**: Updated readme and documentation to reflect the new changes
- 
---

### 0.1.14
- **Fix**: Improved compile feature to work without interupting the Viz renderer. Now creates a dummy scene and uses it to compile the code and give feedback.


### 0.1.13
- **New**: Added feature to compile code on Viz Engine and get feedback in Vs Code.
- **New**: Option `vizscript.enableAutoCompleteHost` - Enable Auto Complete functionality
- **New**: Option `vizscript.enableSignatureHelp` - Enable Signature Help for both built-in and custom procedures
- **New**: Option `vizscript.enableDefinition` - Enable Jump to Definition for easy navigation
- **New**: Option `vizscript.compiler.hostName` - The hostname for connection to Viz Engine
- **New**: Option `vizscript.compiler.hostPort` - The port number for connection to Viz Engine

---

### 0.1.12
- **Fix**: Fixed bug were Function and Sub parameters would show up in wrong scopes while writing new functions.

### 0.1.11

- **Fix**: Further improvements on completions. Fixed bug with overloading for document symbols. Now has full overload support for all procedures.
- **Fix**: Added extra check to remove leading "(" on completion strings 

### 0.1.10
- **Change**: Major improvements on Completion suggestions. Now supports nesting, parantheses and brackets. 
- **Change**: Small adjustments to Syntax Highlighting to highlight important types in all contexts.

### 0.1.9
- **Fix**: Fixed small bug were document scope didn't work for all completions.

### 0.1.8
- **New**: Added configuration settings to turn features on and off.

### 0.1.7
- **Change**: Added different commit characters for procedures and types. Fixed a small bug in syntax highlighting.

### 0.1.6
- **New**: Added classic Viz3 color scheme and a new custom one
- **Change**: Refined syntax highlighting to better support all types
- **Change**: Refined how Global Events are completed

### 0.1.5
- **Change**: Added configuration recommendation to readme
- **Change**: Updated SignatureHelp GIF

### 0.1.4
- **New**: Added demo gifs to Readme

### 0.1.3
- **Change**: Improved completion items suggested by the plugin in different contexts
- **Fix**: Fixed some strange syntax highlighting

### 0.1.2
- **Fix**: Fixed bug where parameters were not showing up in Auto Complete inside functions

### 0.1.1
- **Change**: Renamed configuration settings as they are not yet implemented.

### 0.1.0
- Initial beta release