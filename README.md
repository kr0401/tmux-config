# tmux-config
#   General                
Notes  
- Commands beginning with 'tmux' are from command line  
- Commands beginning with 'C-b' are tmux short cuts, if followed by ':' it's a tmux command
  
Prefix Key
- Used for tmux short cuts and commands
- Control + b (C-b)
  
#   Basics                  
Create unnamed session  
- tmux
- tmux new
- tmux new-session
- C-b :new
  
Create a named session  
- tmux new -s session_name
  
Attach to last session  
- tmux a
- tmux at
- tmux attach
- tmux attach-session
  
Attach to named session  
- tmux a -t session_name
- tmux at -t sessions_name
- tmux attach -t session_name
- tmux attach-session -t session_name
  
Detach from session  
- C-b d
  
Kill session  
- C-b :kill-session
  
Kill named session  
- tmux kill-session -a -t session_name
  
Kill all sessions except current  
- tmux kill-session -a
  
Rename session  
- C-b $
  
List sessions  
- tmux ls
- C-b s
  
#   Windows                  
Create new window  
- C-b c
  
Next window  
- C-b n
  
Previous window  
- C-b p
  
Select window by number  
- C-b 0-9
  
Kill current window  
- C-b &
  
#   Panes                    
Split vertical  
- C-b %
- C-b -
  
Split horizontal  
- C-b "
- C-b |
  
Close current pane  
- C-b x
  
Navigate / switch panes  
- C-b arrow_key
  
Move pane left  
- C-b {
  
Move pane right  
- C-b }
  
Resize pane  
- C-b Alt + arrow_key
  
Auto resize panes (split even)  
- C-b spacebar
  
#   Copy mode                
Enter copy mode  
- C-b [
  
Enter visual (selection) mode  
- v
  
Make selection  
- Arrow keys
- h,j,k,l
- G (go to bottom)
  
Copy (yank) selection  
- y
  
Paste selection  
- C-b P
