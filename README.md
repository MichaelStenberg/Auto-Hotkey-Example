# Auto-Hotkey-Example
#An Auto-Hotkey example/test that can be used to either paste output from the system (which includes the RAW flag for entering to cmd.exe or other command lines) or sending input one line at a time and can include a wait period for the prompt to come back.


SetKeyDelay of -1
^!k::  ; Control+Alt+K hotkey

Clipboard =
(
Clipboard output here.  It can then take what you pre-create to then paste into the CLI of a cmd.exe window which can include programs beyond just cmd.exe but Putty or other tools so it helps as a cross platform reference.

)
SendInput {Raw}%clipboard%

Return

Return


SetKeyDelay of -1
^!l::  ; Control+Alt+L hotkey

Sendinput {Raw}username
Send, {enter}
Sleep, 250
Sendinput {Raw}password
Send, {enter}

Return

Return

