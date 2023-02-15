# bitwarden-at
Small kickoff|bemenu|dmenu|rofi bitwarden autotype script

Inspired from [keepmenu](https://github.com/firecat53/keepmenu) & [bitwarden-menu](https://github.com/firecat53/bitwarden-menu) Needed something faster than the official bw cli. 

Uses [rbw](https://github.com/doy/rbw)-unofficial bitwarden cli, with [PR93](https://github.com/doy/rbw/pull/93) to allow for multiple profiles, and [kickoff](https://github.com/j0ru/kickoff) - a dmenu/bemenu/rofi like launcher written in rust. (Although bemenu/dmenu/rofi could be used.)


After installing rbw and applying the patch in PR93. The RBW_Profile=\<profileName\> env variable can be set. 
With the variable set, running the "rbw config set" commands will save your profile settings in ~/.config/rbw-\<profileName\>

Always specify the \<profileName\> when calling the script - ex: "bw-at personal" or "bw-at work"
The RBW_Profile variable will then be set. Bind it to a shortcut!

Allows to autotype username and password into browser logins, select and type individual entries, and select and type totp codes.
Unable to add entries. rbw allows to add entries but does not seem to sync them to the server.

Works well with [anypinentry](https://github.com/fictitiousexistence/any-pinentry) forked and modified for use with kickoff.
Kickoff allows the password prompt to disable over full screen apps in sway :)
_
[kickoff](https://github.com/j0ru/kickoff) works really well and even displays in sway over fullscreen apps without still being shown on the lock screen. 




