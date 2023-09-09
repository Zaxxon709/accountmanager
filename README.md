# Account Manager

An add-on to make the painful task of authorizing numerous add-ons effortless. Pair multiple service(s) with supported add-ons via a single authorization point and easily manage the data for these service(s).<br><br>


### 709 Repository
[![Download Repo](https://img.shields.io/badge/Download-Repo-blue.svg?style=for-the-badge)](https://raw.githubusercontent.com/Zaxxon709/nexus/main/repository.709-1.0.zip)<br>

### Instructions for adding this repo in Kodi:

<ul>
    <li>Open the Kodi File Manager</li>
    <li>Select "Add source"</li>
    <li>The path for the source is <code>https://zaxxon709.github.io/repo/</code> (Give it the name "709REPO")</li>
</ul>  


### How the addon works:
- Once authorization is complete a check is done for each supported addon to confirm if the addon is installed and if settings.xml exists for that addon.
- If both of these checks are true your Trakt & Debrid data is retrieved from Account Manager and applied to the supported addons.
- During the authorization process a one time backup is also performed to save all Trakt & Debrid data to the default backup directory.<br>


### Support for Custom API Keys:
- Support has been added for your own Custom Trakt API keys. If you have your own keys, please use them. If you do not have keys then head on over to the Trakt website using the link below and create them.<br>

<code>https://trakt.tv/oauth/applications/new</code>


### Note for users/builders:
- For Account Manager to function correctly you need to ensure the directories containing the settings.xml for each supported addon are present in the addon_data directory.
- Some addons do not create the settings.xml after installation. To create it the user first has to open the addon settings menu and then choose 'ok' for the file to be created. If it's not present Account Manager simply does nothing and moves on to the next addon. So, make sure to add these to your build.
- You'll find the option to use Custom Trakt API keys in the add-ons settings menu. I would appreciate it if builders would add their own keys to Account Manager prior to uploading their builds.<br>


### Backup/Restore Data:

- The options to backup, restore and clear data can be found in Account Manager's settings menu.
- The backup created during authorization only backs up current installed add-ons. If you decide to add additional supported addons you should create another backup to save data for those add-ons.<br>
- The default path is not persistent after build updates or fresh starts. For builders i'd recommend your wizard data path for backups. For users i'd recommend whitelisting your backup directory. If the default path is changed make sure to complete another backup.<br>
- The default backup path can also be changed by the user at any time via the Account Manager settings menu.<br>

<p>Default Backup Path = special://userdata/addon_data/plugin.program.accountmgr/</p>


### Restore all Add-ons to Default:
<ul>
    <li>WARNING! Use only to restore system to default settings.</li>
    <li>Open Account Manager and Navigate to the ‘Advanced’ category.
    <li>Select ‘Restore Default Settings'</li>
    <li>This action will delete all your saved data, revoke all add-ons and reset all supported add-ons back to default.</li><br>
</ul>


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


### How to Sync Furk/Easynews/FilePursuit and Metadata:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and add your data into the appropriate field(s)</li>
    <li>Choose 'Sync Add-ons' to sync your data with installed Add-ons</li><br>
</ul>


### Authorize Built-in Commands:

<p>Real-Debrid<br>
RunScript(script.module.accountmgr, action=realdebridAuth)</p>

<p>Premiumize<br>
RunScript(script.module.accountmgr, action=premiumizeAuth)</p>

<p>AllDebrid<br>
RunScript(script.module.accountmgr, action=alldebridAuth)</p>

<p>Trakt<br>
RunScript(script.module.accountmgr, action=traktAuth)</p>

<p>TMDb<br>
RunScript(script.module.accountmgr, action=tmdbAuth)</p><br>


### Sync Built-in Commands:<br>

<p>Real-Debrid<br>
RunScript(script.module.accountmgr, action=realdebridReSync)</p>

<p>Premiumize<br>
RunScript(script.module.accountmgr, action=premiumizeReSync)</p>

<p>AllDebrid<br>
RunScript(script.module.accountmgr, action=alldebridReSync)</p>

<p>Trakt<br>
RunScript(script.module.accountmgr, action=traktReSync)</p>

<p>Sync Multiple Debrid Accounts<br>
RunScript(script.module.accountmgr, action=ReSyncAll)</p>

<p>Sync Furk/Easynews/FilePursuit Accounts<br>
RunScript(script.module.accountmgr, action=SyncAll)</p>

<p>Sync Metadata Accounts<br>
RunScript(script.module.accountmgr, action=metaSync)</p><br>


### View Authorized Add-ons Built-in Commands:<br>

- This allows the user to view what addons are currently authorized

<p>Real-Debrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=realdebrid,return)</p>

<p>Premiumize<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=premiumize,return)</p>

<p>AllDebrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=alldebrid,return)</p>

<p>Trakt<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=trakt,return)</p>

<p>View Multiple Debrid Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=allaccts,return)</p>

<p>View Furk/Easynews/FilePursuit Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=nondebrid,return)</p>

<p>View Metadata Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=metadata,return)</p><br>


### Supported Services:

1.  Real-Debrid<br>
2.  Premiumize<br>
3.  All-Debrid<br>
4.  Trakt<br>
5.  Furk<br>
6.  Easynews<br>
7.  FilePursuit<br>
8.  Fanart.TV<br>
9.  OMDb<br>
10. MDbList<br>
11. IMDb<br>
12. TMDb<br>
13. TVDb<br>


### Debrid Supported Addons:

1.  Seren<br>                   
2.  Fen<br>                   
3.  Ezra<br>
4.  Coalition<br>
5.  POV<br>                     
6.  Umbrella<br>             
7.  Shadow<br>               
8.  Ghost<br>
9.  Base19<br>                  
10. Unleashed<br>             
11. Chain Reaction<br> 
12. Twisted<br>
13. Magic Dragon<br>
14. Asgard<br>
15. Patriot<br>
16. Black Lightning<br>
17. M.E.T.V<br>
18. Aliunde K19<br>
19. My Accounts<br>
20. ResolveURL


### Trakt Supported Addons:
                  
1.  Seren (Custom Trakt API Keys Only)<br>
2.  Fen<br>
3.  Ezra<br>
4.  Coalition<br>
5.  POV<br>                   
6.  Umbrella<br>
7.  Shadow<br>
8.  Ghost<br>
9.  Base19<br>
10. Unleashed<br>            
11. Chain Reaction<br>
12. Magic Dragon<br>
13. Asgard<br>
14. Patriot<br>
15. Black Lightning<br>
16. Aliunde K19<br>
17. Homelander<br> 
18. Quicksilver<br>
19. Chains Genocide<br> 
20. Absolution<br>        
21. Shazam<br>
22. The Crew<br>              
23. Nightwing<br> 
24. Alvin<br>
25. Moria<br>
26. 9 Lives<br>
27. Scrubs V2<br>
28. TMDb Helper<br>
29. Trakt Add-on<br>
30. My Accounts


### Metadata Supported Addons:

1.  Seren<br>                  
2.  Fen<br>
3.  Ezra<br>
4.  Coalition<br>
5.  POV<br>                   
6.  Umbrella<br>
7.  The Crew<br> 
8.  Homelander<br> 
9.  Quicksilver<br>
10. Chains Genocide<br>           
11. Shazam<br>
12. Nightwing<br>
13. Alvin<br>
14. Moria<br>
15. Absolution<br>
16. 9 Lives<br>
17. TMDb Helper<br>
18. Embuary Info<br>
19. Metahandler<br>
20. PVR Artwork Module<br>
21. My Accounts


### Furk Supported Addons:

1.  Fen<br>
2.  Ezra<br>
3.  Coalition<br>
4.  POV<br>
5.  Umbrella<br>
6.  The Crew<br>
7.  Homelander<br>
8.  Quicksilver<br>
9.  Chains Genocide<br>
10. Shazam<br>
11. Nightwing<br>
12. Alvin<br>
13. Moria<br>
14. Absolution<br>
15. 9 Lives<br>
16. My Accounts


### Easynews Supported Addons:

1.  Fen<br>
2.  Ezra<br>
3.  Coalition<br>
3.  POV<br>
4.  Umbrella<br>
5.  The Crew<br>
6.  My Accounts


### FilePursuit Supported Addons:

1.  Umbrella