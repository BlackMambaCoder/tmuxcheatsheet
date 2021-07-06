
# Start

## New session

    tmux

## New named session

    tmux new -s mySession

## List sessions

    tmux ls

## Attach to existing session

    tmux attach -t mySession
    tmux attach -t 13 # if the session is created without a name, it gets a number

## Windows (tabs)

    ctrl+b c        New tab
    ctrl+b ,        Name tab
    ctrl+b &        Kill tab
    ctrl+b :        Setting         E.g.: set mouse => enable mouse for scrolling or clicking
    ctrl+b %        Split vertical (creates only new pane)
    ctrl+b "        Split horizontally (creates only new pane)
    ctrl+b d        Detach, but not close/kill

## Pane

    ctrl+b x        Close (kill) pane
    ctrl+b z        Zoom pane -> "converts" pane into window and backwards

### Move two panes to a new window (tab)

    Enter settings (ctrl+b :)
    Enter "break-pane" 		Moves the pane to a new window

    Go back to your window where the other pane is (be in that pane)
    Enter settings again
    Enter "join-pane -t0:1"	Moves the current pane from session "0" to the new window "1"

## General commands

    ctrl+b t        Show clock
    ctrl+b ?        Show list of commands
    ctrl+b :        Prompt (for settings)

---

## Reference

https://gist.github.com/MohamedAlaa/2961058
