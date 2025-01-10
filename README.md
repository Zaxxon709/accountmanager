# Account Manager

An add-on to make the painful task of authorizing numerous add-ons effortless. Pair multiple service(s) with supported add-ons via a single authorization point and easily manage the data for these service(s).<br><br>


### 709 Repository
[![Download Repo](https://img.shields.io/badge/Download-Repo-blue.svg?style=for-the-badge)](https://raw.githubusercontent.com/Zaxxon709/nexus/main/repository.709-1.0.zip)<br>

### Instructions for adding this repo in Kodi:

<ul>
    <li>Open the Kodi File Manager</li>
    <li>Select "Add source"</li>
    <li>The path for the source is <code>https://zaxxon709.github.io/repo/</code> (Give it the name "709REPO")</li><br>
</ul>  


### Custom Trakt API Key Section for Users:
- If you have your own Trakt API keys, please use them.<br> 
- Open Account Manager's settings menu and navigate to the Accounts section to enable this feature and enter your keys<br>
- If you do not already have keys then just follow the link below to create them.<br>
IMPORTANT: If you have previously authorized Trakt via Account Manager but now wish to use your own Trakt API keys then you must revoke your current authorizations before applying your own custom keys.<br>

<code>https://trakt.tv/oauth/applications/new</code><br>


### Custom Trakt API Key Section for Builders:
- Builders can add their own custom keys in this section.<br>
- Open Account Manager's settings menu and naviagte to the Advanced section to enable this feature and enter your keys.<br>
- Keys added here are obfuscated using asterisks and are persistent after add-on updates/revokes.<br>
- If you do not already have keys then just follow the link below to create them.<br>

<code>https://trakt.tv/oauth/applications/new</code><br>


### Backup/Restore Data:

- The options to backup, restore and clear data can be found in Account Manager's settings menu.
- The backup created during authorization only backs up current installed add-ons. If you decide to add additional supported addons you should create another backup to save data for those add-ons.<br>
- The default path is not persistent after build updates or fresh starts. For builders, I'd recommend your wizard data path for backups.<br>
- The default backup path can be changed any time in Account Manager's settings menu. If the default path is changed make sure to complete another backup.<br>

<p>Default Backup Path = special://userdata/addon_data/plugin.program.accountmgr/</p>


### Restore all Add-ons to Default:
<ul>
    <li>Use ONLY to restore all add-ons to default settings prior to using Account Manager.</li>
    <li>Open Account Manager and Navigate to the ‘Advanced’ category.</li>
    <li>Select ‘Restore Default Settings'</li>
    <li>This action will revoke all services, reset all add-on settings back to default, and delete all your saved data</li>
</ul>


### Supported Services:

1.  Trakt<br>
2.  Real-Debrid<br>
3.  Premiumize<br>
4.  All-Debrid<br>
5.  TorBox<br>
6.  Easy Debrid<br>
7.  OffCloud
8.  Easynews<br>
9.  FilePursuit<br>
10. Fanart.TV<br>
11. OMDb<br>
12. MDbList<br>
13. IMDb<br>
14. TMDb<br>
15. TVDb<br><br>



### Open Account Manager:

<p>RunAddon(script.module.accountmgr)</p><br>


### Authorize:<br>

<p>Trakt<br>
RunScript(script.module.accountmgr, action=traktAuth)</p>

<p>Real-Debrid<br>
RunScript(script.module.accountmgr, action=realdebridAuth)</p>

<p>Premiumize<br>
RunScript(script.module.accountmgr, action=premiumizeAuth)</p>

<p>AllDebrid<br>
RunScript(script.module.accountmgr, action=alldebridAuth)</p>

<p>TorBox<br>
RunScript(script.module.accountmgr, action=torboxAuth)</p>

<p>Easy Debrid<br>
RunScript(script.module.accountmgr, action=easydebridAuth)</p>

<p>OffCloud<br>
RunScript(script.module.accountmgr, action=offcloudAuth)</p>

<p>Easynews<br>
RunScript(script.module.accountmgr, action=easynewsAuth)</p>

<p>Filepursuit<br>
RunScript(script.module.accountmgr, action=filepursuitAuth)</p>

<p>TMDb<br>
RunScript(script.module.accountmgr, action=tmdbAuth)</p><br>


### Sync:<br>

<p>Trakt<br>
RunScript(script.module.accountmgr, action=traktReSync)</p>

<p>Real-Debrid<br>
RunScript(script.module.accountmgr, action=realdebridReSync)</p>

<p>Premiumize<br>
RunScript(script.module.accountmgr, action=premiumizeReSync)</p>

<p>AllDebrid<br>
RunScript(script.module.accountmgr, action=alldebridReSync)</p>

<p>Sync Multiple Debrid Accounts<br>
RunScript(script.module.accountmgr, action=ReSyncAll)</p>

<p>TorBox<br>
RunScript(script.module.accountmgr, action=torboxReSync)</p>

<p>Easy Debrid<br>
RunScript(script.module.accountmgr, action=easydebridReSync)</p>

<p>OffCloud<br>
RunScript(script.module.accountmgr, action=offcloudReSync)</p>

<p>Easynews<br>
RunScript(script.module.accountmgr, action=easynewsReSync)</p>

<p>FilePursuit<br>
RunScript(script.module.accountmgr, action=filepursuitReSync)</p>

<p>Metadata<br>
RunScript(script.module.accountmgr, action=metaReSync)</p><br>


### View Authorized Addons:<br>

<p>Trakt<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=trakt,return)</p>

<p>Real-Debrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=realdebrid,return)</p>

<p>Premiumize<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=premiumize,return)</p>

<p>AllDebrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=alldebrid,return)</p>

<p>View Multiple Debrid Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=allaccts,return)</p>

<p>TorBox<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=torbox,return)</p>

<p>Easy Debrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=easydebrid,return)</p>

<p>OffCloud<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=offcloud,return)</p>

<p>Easynews<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=easynews,return)</p>

<p>FilePursuit<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=filepursuit,return)</p>

<p>View Metadata Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=metadata,return)</p><br>



### Supported Addons:

### Debrid

1.  Seren<br>                   
2.  Fen<br>
3.  Fen Light<br>               
4.  The Coalition<br>
5.  POV<br>                     
6.  Umbrella<br>
7.  Infinity<br>
8.  Dradis<br>        
9.  Shadow<br>              
10. Ghost<br>
11. Base<br>                            
12. Chain Reaction<br>
13. Asgard<br>
14. Patriot<br>
15. Black Lightning<br>
16. M.E.T.V<br>
17. Aliunde 19<br>
18. Nightwing Lite<br>
19. Chains Genocide<br>
20. Otaku<br>
21. Realizer<br>
22. Premiumizer<br>
23. All Accounts<br>
24. My Accounts<br>
25. ResolveURL	


### TorBox

1. Fen Light<br>
2. Umbrella<br>
3. POV<br>
4. Infinity<br>
5. Dradis<br>
6. Otaku


### Easy Debrid

1. Fen Light<br>
2. Umbrella<br>
3. POV<br>
4. Infinity<br>
5. Dradis


### OffCloud

1. Fen Light<br>
2. Umbrella<br>
3. POV<br>
4. Infinity<br>
5. Dradis


### Trakt
                  
1.  Seren (Custom Trakt API Keys Only)<br>
2.  Fen<br>
3.  Fen Light<br>
4.  The Coalition<br>
5.  POV<br>                  
6.  Umbrella<br>
7.  Infinity<br>
8.  Dradis<br>
9.  Shadow<br>
10. Ghost<br>
11. Base<br>         
12. Chain Reaction<br>
13. Asgard<br>
14. Patriot<br>
15. Black Lightning<br>
16. Aliunde K19<br>
17. Nightwing Lite<br>
18. Homelander<br>
19. Quicksilver<br>
20. Chains Genocide<br>
21. Absolution<br>      
22. Shazam<br>
23. The Crew<br>              
24. Alvin<br>
25. Moria<br>
26. Nine Lives<br>
27. Scrubs V2<br>
28. TMDb Helper<br>
29. Trakt Add-on<br>
30. All Accounts<br>
31. My Accounts


### Easynews

1.  Fen<br>
2.  Fen Light<br>
3.  The Coalition<br>
4.  POV<br>
5.  Umbrella<br>
6.  Infinity<br>
7.  Dradis<br>
8.  The Crew<br>
9.  All Accounts<br>
10. My Accounts


### FilePursuit

1. Umbrella<br>
2. Infinity<br>
3. Dradis<br>
4. All Accounts<br>
5. My Accounts


### Metadata

1.  Seren <br>                 
2.  Fen<br>
3.  Fen Light<br>
4.  The Coalition<br>
5.  POV<br>                   
6.  Umbrella<br>
7.  Infinity<br>
8.  Dradis<br>
9.  The Crew<br> 
10. Homelander<br> 
11. Quicksilver<br>
12. Chains Genocide<br>           
13. Shazam<br>
14. Nightwing Lite<br>
15. Alvin<br>
16. TheLab<br>
17. Moria<br>
18. Absolution<br>
19. Nine Lives<br>
20. TMDb Helper<br>
21. Embuary Info<br>
22. Metahandler<br>
23. PVR Artwork Module<br>
24. All Accounts<br>
25. My Accounts<br>
26. Fentastic Skin<br>
27. Nimbus Skin