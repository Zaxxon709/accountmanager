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
15. Aliunde<br>
16. Adina<br>
17. Artemis<br>
18. Dynasty<br>
19. Loonatics Empire<br>
20. Premiumizer<br>
21. Realizer<br>
22. Your Accounts<br>
23. My Accounts<br>
24. ResolveURL


### Trakt Supported Addons:
                  
1.  Ezra<br>
2.  Fen<br>
3.  POV<br>                   
4.  Umbrella<br>
5.  Shadow<br>
6.  Ghost<br>
7.  Unleashed<br>            
8.  Chain Reaction<br>
9.  Base 19<br> 
10. Magic Dragon<br>
11. Asgard<br>
12. Patriot<br>
13. Homelander<br> 
14. Quicksilver<br>
15. Chains Genocide<br>           
16. Shazam<br>
17. The Promise<br>
18. The Crew<br>              
19. Nightwing<br> 
20. Alvin<br>
21. Moria<br>
22. Nine Lives<br>
23. Scrubs V2<br>
24. TMDb Helper<br>
25. Trakt Add-on<br>
26. My Accounts


### Metadata Supported Addons:

1.  Seren<br>                  
2.  Ezra<br>
3.  Fen<br>
4.  POV<br>                   
5.  Umbrella<br>
6.  Adina<br>
7.  Artemis<br>
8.  Dynasty<br>
9.  Loonatics Empire<br>
10. The Crew<br> 
11. Homelander<br> 
12. Quicksilver<br>
13. Chains Genocide<br>           
14. Shazam<br>
15. The Promise<br>
16. Nightwing<br>
17. Alvin<br>
18. Moria<br>
19. Nine Lives<br>
20. TMDb Helper<br>
21. Embuary Info<br>
22. Metahandler<br>
23. PVR Artwork Module<br>
24. Your Accounts<br>
25. My Accounts


### Furk Supported Addons:

1.  Ezra<br>
2.  Fen<br>
3.  POV<br>
4.  Umbrella<br>
5.  Adina<br>
6.  Artemis<br>
7.  Dynasty<br>
8.  Lonnatics Empire<br>
9.  The Crew<br>
10. Homelander<br>
11. Quicksilver<br>
12. Chains Genocide<br>
13. Shazam<br>
14. The Promise<br>	
15. Nightwing<br>
16. Alvin<br>
17. Moria<br>
18. Nine Lives<br>
19. Your Accounts<br>
20. My Accounts


### Easynews Supported Addons:

1.  Ezra<br>
2.  Fen<br>
3.  POV<br>
4.  Umbrella<br>
5.  Adina<br>
6.  Artemis<br>
7.  Dynasty<br>
8.  The Crew<br>
9.  Your Accounts<br>
10. My Accounts


### FilePursuit Supported Addons:

1.  Umbrella<br>
2.  Artemis<br>
3.  Dynasty<br>
4.  Your Accounts<br>
5.  My Accounts