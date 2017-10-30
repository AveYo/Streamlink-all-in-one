#### Streamlink all-in-one package
The included MPC-HC video player uses pass-trough and gpu hw acceleration with low resources usage  
Use Middle DblClick to reload stream in MPC-HC if any issues, Left DblClick to switch Fullscreen   
Refactored to hide the command window at launch, show gui dialogs for URL and STREAM as needed  
Detects options like --help or --twitch-oauth-authenticate in url input-dialog and shows cmd window    

![Preview](streamlink_preview.png)  

#### EXAMPLE USAGE  
Unzip & run `dreamleague.bat` or `dreamleague+chat.bat`  
~ __a dialog will ask to select stream quality__  
~ video will play in MPC-HC (included), Twitch chat will start in a browser tab (only for +chat variant)  
Create new batch scripts for your favourite Twitch streams by simply making a copy of an example batch file then rename it to the twitch stream name i.e. `dreamleague.bat` to `moonducktv.bat`  
  
#### COMMAND-LINE USAGE  
After first launch, `streamlink\streamlink.bat` can be called from any path or [Win+R] run menu:  
STREAMLINK                                             _= with no parameters shows stream name input-dialog_   
STREAMLINK dreamleague  _= with just the url or twitch channel name shows quality choice-dialog_    
STREAMLINK twitch.tv/dreamleague 720p _= with both url + quality launches video player directly_   
  
#### PLUGIN USAGE:   
Get _'Open With'_ plugin for firefox - https://addons.mozilla.org/en-US/firefox/addon/open-with/  
_'Open With Options'_ - _'Add'_ - set filter _'Applications'_ to _'All files'_ - browse to `streamlink\streamlink.bat`  
Now you can directly right-click stream link in firefox and choose _'Open Link with -- streamlink.bat'_  
