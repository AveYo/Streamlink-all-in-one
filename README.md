#### Streamlink all-in-one package for Windows v9f  
The included MPC-HC video player uses pass-trough and gpu hw acceleration with low resources usage  
Use Middle DblClick to reload stream in MPC-HC if any issues, Left DblClick to switch Fullscreen   
Refactored to hide the command window at launch, show gui dialogs for URL and STREAM as needed  
Added `streamlink\Setup_Open_With_Firefox_and_Chrome_Addon.bat` with detailed instructions  
Updated MPC-HC and Streamlink binaries [2018.06.24]

[Dialogs preview](https://github.com/AveYo/Streamlink-all-in-one/blob/master/streamlink_preview.png?raw=true)
  
#### EXAMPLE USAGE  
Unzip & run `dreamleague.bat` or `dreamleague+chat.bat`  
~ __a dialog will ask to select stream quality__  
~ video will play in MPC-HC (included), Twitch chat will start in a browser tab (only for +chat variant)  
Create new batch scripts for your favourite Twitch streams by simply making a copy of an example batch file  
then rename it to the twitch stream name i.e. `dreamleague.bat` to `moonducktv.bat`  
  
#### COMMAND-LINE USAGE  
After first launch, `streamlink\streamlink.bat` can be called from any path or [Win+R] run menu:  
~ `streamlink`                             = with no arguments shows url input-dialog   
~ `streamlink dreamleague`                 = with just the url or twitch channel name shows stream choice-dialog   
~ `streamlink dreamleague 720p`  = with both url and stream choice launches video player directly  
~ `streamlink dreamleague+chat`            = with +chat added to the url also opens twitch chat in browser tab    
~ `streamlink --twitch-oauth-authenticate` = with any python options shows cmd window   
  
#### PLUGIN USAGE:   
1: Run `streamlink\Setup_Open_With_Firefox_and_Chrome_Addon.bat`  
once or each time after changing Streamlink-all-in-one location  
2: Get ['Open With' plugin for Firefox](https://addons.mozilla.org/en-US/firefox/addon/open-with/)    
or Get ['Open With' plugin for Chrome](https://chrome.google.com/webstore/detail/open-with/cogjlncmljjnjpbgppagklanlcbchlno)  
3: Launch Firefox or Chrome - 'Open With Options' - [Add browser]:  
~ Name: `Streamlink`  
~ Command: `streamlink.bat`  
~ [Add]  
Optionally [Add browser]:   
~ Name: `Streamlink chat`  
~ Command: `streamlink.bat %s+chat`  
~ [Add]  
Optionally [Add browser]:   
~ Name: `Streamlink 720p`  
~ Command: `streamlink.bat %s 720p`  
~ [Add]  
4: Right click any stream url in Firefox or Chrome   
and select 'Open With' - 'Streamlink' entry to launch it via __streamlink.bat__!  
