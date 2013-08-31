An ignore module for ZNC 1.0.

Build with `znc-buildmod`. Move the resulting `.so` file to your `~/.znc/modules`.

Pull requests welcome.

### Usage

	 Command    | Arguments                     | Description
	------------|-------------------------------|--------------------------------------------------------------------------------
	 AddHost    | [mMaAnNcC] `<nick!user@host>` | Ignore a hostmask from [m]essage, [a]ction, [n]otice, [c]tcp; uppercase = private
	 AddPattern | [mMaAnNcC] `<regex>`          | Ignore text matching a regular expression
	 Clear      |                               | Clear all ignore entries
	 Del        | `<n>`                         | Remove an ignore entry by index
	 Help       | search                        | Generate this output
	 List       |                               | Display the ignore list
	 Unload     |                               | Unload this module

The required arguments for AddHost and AddPattern should be "quoted" if they contain spaces.

### To do

- Ignore invites
- Ignore DCC (I'll have to take a look at how this works in the IRC protocol)
