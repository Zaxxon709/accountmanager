# Account Manager

### How the addon works:
- Once authorization is complete a check is done for each supported addon to confirm if the addon is installed and if settings.xml exists for that addon.
- If both of these checks are true your Trakt & Debrid data is retrieved from Account Manager and applied to the supported addons.
- A backup is then performed to save all Trakt & Debrid data for all authorized add-ons.<br><br>

### Note for users/builders:
- For Account Manager to function correctly you need to ensure the directories containing the settings.xml for each supported addon are present in the addon_data directory
- Some addons do not create the settings.xml after installation. To create it the user first has to open the addon settings menu and then choose 'ok' for the file to be created. If it's not present Account Manager simply does nothing and moves on to the next addon. So, make sure to add these to your build.<br><br>


### How to Authorize Debrid:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to ‘Debrid Accounts’ and choose your debrid service(s)</li>
    <li>Select 'Authorize' and proceed to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and choose 'OK' to exit</li>
    <li>All supported add-ons are now authorized!</li><br>
</ul>


### How to Authorize Trakt:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to ‘Trakt Account’ and select ‘Authorize’ to pair your account</li>
    <li>Once Account Manager authorization is complete the user has two choices on how to authorize their add-ons</li>
</ul>
    1.  Sync All Add-ons – This will sync your Trakt account with all supported add-ons that are currently installed<br>
    2.  Sync Individual Add-ons – Choose add-ons to authorize from the list of supported add-ons<br><br>


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
RunScript(script.module.myaccts, action=traktSync)</p><br>


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

- The default backup path can be changed by the user via the Accounts Manager settings menu

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
13. My Accounts