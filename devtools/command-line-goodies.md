# iTerm additional key bindings

First of all, I advice using [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh) and [iTerm](https://www.iterm2.com/) as a Mac terminal replacement.

To start, open your iTerm, go to `Preferences > Keys` and then click to `+` button to add new key bindings.

**Note:** you can change key configuration by your taste.

#### Delete whole word

- Keys: `⌥`+`⟵(Delete)`
- Action: `Send Hex Code`
  - `0x1B 0x08`
  
#### Delete word forward

- Keys: `⌥`+`fn`+`⟵(Delete)`
- Action: `Send Escape Sequence`
  - Esc + `d`
  
#### Clear whole line

- Keys: `⌘`+`Shift`+`⟵(Delete)`
- Action: `Send Hex Code`
  - `0x15`
  
#### Jump cursor to left over whole word

- Keys: `⌥`+`←`
- Action: `Send Escape Sequence`
  - Esc + `b`
  
#### Jump cursor to right over whole word

- Keys: `⌥`+`→`
- Action: `Send Escape Sequence`
  - Esc + `f`
  
#### Jump cursor to line start

- Keys: `⌘`+`←`
- Action: `Send Hex Code`
  - `0x01`
  
#### Jump cursor to line end

- Keys: `⌘`+`→`
- Action: `Send Hex Code`
  - `0x05`
