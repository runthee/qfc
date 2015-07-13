# qfc
Quick Command-line File Completion

![qfc](https://cloud.githubusercontent.com/assets/2557967/8640880/582cb8fe-28ff-11e5-9753-41464dda938e.gif)

qfc is a shell auto-complete alternative which features real-time multi-directories matching: It matches files while you type against multiple directories, not just the current one.
This is useful, to avoid the burden of writing the whole path whenever you want to `cd` or `vim` a file, which is frequent espacielly if you use the terminal as your IDE(The terminal is the best IDE, remember!).

## Features:
- Real-time matching: Results are displayed while you type.
- Multi-directories && Context relevant matching: if you're in a cvs(git,mercurial) tracked directory, qfc will matches against your tracked(or new) files only. This is very useful to avoid 10000+ of dependency files to clutter up the results. 
- Enhanced Filtering/Sorting of matches.

## Usage:
- Ctrl-f : complete the word under cursor using qfc
- while qfc is open:
    - TAB: Append the selected match to the current path
    - ENTER: Append the selected match to the current path and returns the result
    - Ctrl-f: Returns the current path.
    - Arrows keys: Navigation between directories


## Installation:
- `git clone https://github.com/pindexis/qfc $HOME/.qfc`
- Add the following line to your *.rc :  
    `[[ -s "$HOME/.qfc/bin/qfc.sh" ]] && source "$HOME/.qfc/bin/qfc.sh"`
