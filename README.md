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


### Open Account Manager:

<p>RunAddon(script.module.accountmgr)</p><br>

### Authorize:<br>

<p>Real-Debrid<br>
RunScript(script.module.accountmgr, action=realdebridAuth)</p>

<p>Premiumize<br>
RunScript(script.module.accountmgr, action=premiumizeAuth)</p>

<p>AllDebrid<br>
RunScript(script.module.accountmgr, action=alldebridAuth)</p>

<p>OffCloud<br>
RunScript(script.module.accountmgr, action=offcloudAuth)</p>

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

<p>OffCloud<br>
RunScript(script.module.accountmgr, action=offcloudReSync)</p>

<p>Trakt<br>
RunScript(script.module.accountmgr, action=traktReSync)</p>

<p>Sync Multiple Debrid Accounts<br>
RunScript(script.module.accountmgr, action=ReSyncAll)</p>

<p>Easynews<br>
RunScript(script.module.accountmgr, action=easynewsReSync)</p>

<p>FilePursuit<br>
RunScript(script.module.accountmgr, action=filepursuitReSync)</p>

<p>Metadata<br>
RunScript(script.module.accountmgr, action=metaReSync)</p><br>


### View Authorized Addons:<br>

<p>Real-Debrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=realdebrid,return)</p>

<p>Premiumize<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=premiumize,return)</p>

<p>AllDebrid<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=alldebrid,return)</p>

<p>OffCloud<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=easynews,return)</p>

<p>Trakt<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=trakt,return)</p>

<p>View Multiple Debrid Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=allaccts,return)</p>

<p>Easynews<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=easynews,return)</p>

<p>FilePursuit<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=filepursuit,return)</p>

<p>View Metadata Accounts<br>
ActivateWindow(10001,plugin://script.module.acctview/?mode=metadata,return)</p><br>


### Supported Services:

1.  Real-Debrid<br>
2.  Premiumize<br>
3.  All-Debrid<br>
4.  OffCloud
5.  Trakt<br>
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
9.  Infinity<br>
10. Dradis<br>
11. Taz19<br>            
12. Shadow<br>              
13. Ghost<br>
14. Base<br>                 
15. Unleashed<br>             
16. Chain Reaction<br>
17. Twisted<br>
18. Magic Dragon<br>
19. Asgard<br>
20. Patriot<br>
21. Black Lightning<br>
22. M.E.T.V<br>
23. Aliunde<br>
24. Nightwing Lite<br>
25. Chains Genocide<br>
26. Otaku<br>
27. Realizer<br>
28. Premiumizer<br>
29. All Accounts<br>
30. My Accounts<br>
31. ResolveURL	


### OffCloud

1. POV<br>
2. Dradis


### Trakt
                  
1.  Seren (Custom Trakt API Keys Only)<br>
2.  Fen<br>
3.  Fen Light<br>
4.  afFENity<br>
5.  Ezra<br>
6.  The Coalition<br>
7.  POV<br>                  
8.  Umbrella<br>
9.  Infinity<br>
10. Dradis<br>
11. Taz19<br>
12. Shadow<br>
13. Ghost<br>
14. Base<br>
15. Unleashed<br>           
16. Chain Reaction<br>
17. Magic Dragon<br>
18. Asgard<br>
19. Patriot<br>
20. Black Lightning<br>
21. Aliunde K19<br>
22. Nightwing Lite<br>
23. Homelander<br>
24. Quicksilver<br>
25. Chains Genocide<br>
26. Absolution<br>      
27. Shazam<br>
28. The Crew<br>              
29. Alvin<br>
30. Moria<br>
31. Nine Lives<br>
32. Scrubs V2<br>
33. TMDb Helper<br>
34. Trakt Add-on<br>
35. All Accounts<br>
36. My Accounts


### Easynews

1.  Fen<br>
2.  Fen Light<br>
3.  afFENity<br>
4.  Ezra<br>
5.  The Coalition<br>
6.  POV<br>
7.  Umbrella<br>
9.  Infinity<br>
9.  Dradis<br>
10. Taz19<br>
11. The Crew<br>
12. All Accounts<br>
13. My Accounts


### FilePursuit

1. Umbrella<br>
2. Infinity<br>
3. Dradis<br>
4. All Accounts<br>
5. My Accounts


### Metadata

1.  Seren<br>                  
2.  Fen<br>
3.  Fen Light<br>
4.  afFENity<br>
5.  Ezra<br>
6.  The Coalition<br>
7.  POV<br>                   
8.  Umbrella<br>
9.  Infinity<br>
10. Dradis<br>
11. Taz19<br>
12. The Crew<br> 
13. Homelander<br>
14. Quicksilver<br>
15. Chains Genocide<br>           
16. Shazam<br>
17. Alvin<br>
18. Moria<br>
19. Absolution<br>
20. Nine Lives<br>
21. TMDb Helper<br>
22. Embuary Info<br>
23. Metahandler<br>
24. PVR Artwork Module<br>
25. All Accounts<br>
26. My Accounts