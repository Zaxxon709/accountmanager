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


### Custom Trakt API Keys:
- If you have your own Trakt API keys, please use them.<br> 
- You can enter your keys within Account Manager's settings menu.
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
    <li>WARNING! Use only to restore system to default settings.</li>
    <li>Open Account Manager and Navigate to the ‘Advanced’ category.
    <li>Select ‘Restore Default Settings'</li>
    <li>This action will revoke all services, reset all add-on settings back to default, and delete all your saved data</li>
</ul>


### How to Authorize Debrid:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and choose your debrid service(s)</li>
    <li>Select 'Authorize' and proceed to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and choose 'OK' to exit</li>
    <li>All supported add-ons are now authorized!</li>
</ul>


### How to Authorize Trakt:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and select ‘Authorize’ to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and when prompted choose 'OK' to force close Kodi</li>
    <li>All supported add-ons are now authorized!</li>
</ul>


### How to Sync Furk/Easynews/FilePursuit and Metadata:
<ul>
    <li>Open Account Manager</li>
    <li>Navigate to the ‘Accounts’ category and add your data into the appropriate field(s)</li>
    <li>Choose 'Sync Add-ons' to sync your data with installed Add-ons</li>
    <li>Wait for the 'Sync is complete' notification and when prompted choose 'OK' to force close Kodi</li>
    <li>All supported add-ons are now synced!</li><br>
</ul>


### Open Account Manager:

<p>RunAddon(script.module.accountmgr)</p><br>

### Authorize:<br>

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


### Sync:<br>

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
RunScript(script.module.accountmgr, action=metaReSync)</p><br>


### View Authorized Addons:<br>

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

### Supported Addons:

### Debrid

1.  Seren<br>                   
2.  Fen<br>
3.  Fen Light<br>
4.  afFENity<br>                  
5.  Ezra<br>
6.  The Coalition<br>
7.  POV<br>                     
8.  Umbrella<br>
9.  Dradis<br>
10. Taz19<br>            
11. Shadow<br>              
12. Ghost<br>
13. Base<br>                 
14. Unleashed<br>             
15. Chain Reaction<br>
16. Twisted<br>
17. Magic Dragon<br>
18. Asgard<br>
19. Patriot<br>
20. Black Lightning<br>
21. M.E.T.V<br>
22. Aliunde<br>
23. Otaku<br>
24. Realizer<br>
25. Premiumizer<br>
26. All Accounts<br>
27. My Accounts<br>
28. ResolveURL	


### Trakt
                  
1.  Seren (Custom Trakt API Keys Only)<br>
2.  Fen<br>
3.  Fen Light<br>
4.  afFENity<br>
5.  Ezra<br>
6.  The Coalition<br>
7.  POV<br>                  
8.  Umbrella<br>
9.  Dradis<br>
10. Taz19<br>
11. Shadow<br>
12. Ghost<br>
13. Base<br>
14. Unleashed<br>           
15. Chain Reaction<br>
16. Magic Dragon<br>
17. Asgard<br>
18. Patriot<br>
19. Black Lightning<br>
20. Aliunde K19<br>
21. Homelander<br>
22. TheLab<br>
23. Quicksilver<br>
24. Chains Genocide<br>
25. Absolution<br>      
26. Shazam<br>
27. The Crew<br>              
28. Nightwing<br> 
29. Alvin<br>
30. Moria<br>
31. Nine Lives<br>
32. Scrubs V2<br>
33. TheLabjr<br>
34. TMDb Helper<br>
35. Trakt Add-on<br>
36. All Accounts<br>
37. My Accounts


### Metadata

1.  Seren<br>                  
2.  Fen<br>
3.  Fen Light<br>
4.  afFENity<br>
5.  Ezra<br>
6.  The Coalition<br>
7.  POV<br>                   
8.  Umbrella<br>
9.  Dradis<br>
10. Taz19<br>
11. The Crew<br> 
12. Homelander<br>
13. TheLab<br> 
14. Quicksilver<br>
15. Chains Genocide<br>           
16. Shazam<br>
17. Nightwing<br>
18. Alvin<br>
19. Moria<br>
20. Absolution<br>
21. Nine Lives<br>
22. TMDb Helper<br>
23. Embuary Info<br>
24. Metahandler<br>
25. PVR Artwork Module<br>
26. All Accounts<br>
27. My Accounts


### Furk

1.  Fen<br>
2.  Ezra<br>
3.  The Coalition<br>
4.  POV<br>
5.  Umbrella<br>
6.  Dradis<br>
7.  Taz19<br>
8.  The Crew<br>
9.  Homelander<br>
10. TheLab<br>
11. Quicksilver<br>
12. Chains Genocide<br>
13. Shazam<br>
14. Nightwing<br>
15. Alvin<br>
16. Moria<br>
17. Absolution<br>
18. Nine Lives<br>
19. All Accounts<br>
20. My Accounts


### Easynews

1.  Fen<br>
2.  Fen Light<br>
3.  afFENity<br>
4.  Ezra<br>
5.  The Coalition<br>
6.  POV<br>
7.  Umbrella<br>
8.  Dradis<br>
9.  Taz19<br>
10. The Crew<br>
11. All Accounts<br>
12. My Accounts


### FilePursuit

1. Umbrella<br>
2. Dradis<br>
3. All Accounts<br>
4. My Accounts