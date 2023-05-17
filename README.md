# Account Manager

### How the addon works:
- Once authorization is complete a check is done for each supported addon to confirm if the addon is installed and if settings.xml exists for that addon.
- If both of these checks are true your Trakt & Debrid data is retrieved from Account Manager and applied to the supported addons.
- During the authorization process a one time backup is performed to save all Trakt & Debrid data to the default backup directory.<br><br>

### Note for users/builders:
- For Account Manager to function correctly you need to ensure the directories containing the settings.xml for each supported addon are present in the addon_data directory
- Some addons do not create the settings.xml after installation. To create it the user first has to open the addon settings menu and then choose 'ok' for the file to be created. If it's not present Account Manager simply does nothing and moves on to the next addon. So, make sure to add these to your build.<br><br>


### How to Authorize Debrid:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and choose your debrid service(s)</li>
    <li>Select 'Authorize' and proceed to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and choose 'OK' to exit</li>
    <li>All supported add-ons are now authorized!</li><br>
</ul>


### How to Authorize Trakt:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and select ‘Authorize’ to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and when prompted choose 'OK' to force close Kodi</li>
    <li>All supported add-ons are now authorized!</li><br>
</ul>


### Authorize Built-in Commands:

<p>Real-Debrid<br>
RunScript(script.module.myaccts, action=realdebridAuth)</p>

<p>Premiumize<br>
RunScript(script.module.myaccts, action=premiumizeAuth)</p>

<p>AllDebrid<br>
RunScript(script.module.myaccts, action=alldebridAuth)</p>

<p>Trakt<br>
RunScript(script.module.myaccts, action=traktAuth)</p><br>


### Revoke All Add-ons Built-in Commands:

<p>Real-Debrid<br>
PlayMedia(plugin://script.module.myauth/?mode=addondebrid_rd&name=all)</p>

<p>Premiumize<br>
PlayMedia(plugin://script.module.myauth/?mode=addondebrid_pm&name=all)</p>

<p>AllDebrid<br>
PlayMedia(plugin://script.module.myauth/?mode=addondebrid_ad&name=all)</p>

<p>Trakt<br>
PlayMedia(plugin://script.module.myauth/?mode=addontrakt&name=all)</p><br>


### Sync All Add-ons Built-in Commands:<br>

<p>Real-Debrid<br>
RunScript(script.module.myaccts, action=realdebridSync)</p>

<p>Premiumize<br>
RunScript(script.module.myaccts, action=premiumizeSync)</p>

<p>AllDebrid<br>
RunScript(script.module.myaccts, action=alldebridSync)</p>

<p>Trakt<br>
RunScript(script.module.myaccts, action=traktReSync)</p><br>


### View Your Authorized Add-ons Built-in Commands:<br>

- This allows the user to view what addons are currently authorized

<p>Real-Debrid<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=realdebrid,return)</p>

<p>Premiumize<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=premiumize,return)</p>

<p>AllDebrid<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=alldebrid,return)</p>

<p>Trakt<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=trakt,return)</p><br>


### Backup Trakt & debrid Data:

- During authorization of your Trakt or Debrid account a one time backup is completed to save your data for all add-ons
- The default backup path can be changed at any time by the user via the Account Manager settings menu. For builders i'd recommend your wizard data path for backups
- If the path is changed make sure to complete another backup

<p>Default Backup Path<br>
special://userdata/addon_data/script.module.myaccts/</p><br>


### Supported Debrid Addons:

1.  Seren<br>                   
2.  Ezra<br>                    
3.  Fen<br>
4.  POV<br>                     
5.  Umbrella<br>             
6.  Shadow<br>               
7.  Ghost<br>                  
8.  Unleashed<br>             
9.  Chain Reaction<br> 
10. Twisted<br>
11. Base19<br>
12. Magic Dragon<br>
13. Asgard<br>
14. M.E.T.V<br>
15. Premiumizer<br>
16. Realizer<br>
17. My Accounts<br>
18. ResolveURL


### Supported Trakt Addons:

1.  TMDb Helper<br>
2.  Trakt Add-on<br> 
3.  Seren<br>                   
4.  Ezra<br>
5.  Fen<br>
6.  POV<br>                   
7.  Umbrella<br>             
8.  Homelander<br>               
9.  The Crew<br>                  
10. Shazam<br>             
11. Nightwing<br> 
12. The Promise<br>
13. Alvin<br>
14. Scrubs V2<br>
13. My Accounts