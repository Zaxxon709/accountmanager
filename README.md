# Account Manager Lite

A utility designed to centralize the authorization of various third-party streaming services across multiple Kodi add-ons. It simplifies setup by allowing users to enter account credentials once rather than in each add-on individually.

### 709 Repository
[![Download Repo](https://img.shields.io/badge/Download-Repo-blue.svg?style=for-the-badge)](https://raw.githubusercontent.com/Zaxxon709/nexus/main/repository.709-1.0.2.zip)<br>

### Instructions for adding this repo in Kodi:

<ul>
    <li>Open the Kodi File Manager</li>
    <li>Select "Add source"</li>
    <li>The path for the source is <code>https://zaxxon709.github.io/repo/</code> (Give it the name "709REPO")</li><br>
</ul>  


### Supported Services:


1.  Trakt<br>
2.  MDBList<br>
3.  Real-Debrid<br>
4.  Premiumize<br>
5.  All-Debrid<br>
6.  TorBox<br>
7.  OffCloud<br>
8.  Easynews<br><br>


### Open Account Manager Lite:

RunAddon(script.module.acctmgr)<br>


### View Account Info:

RunScript(script.module.acctmgr, action=traktAcct)<br>
RunScript(script.module.acctmgr, action=realdebridAcct)<br>
RunScript(script.module.acctmgr, action=premiumizeAcct)<br>
RunScript(script.module.acctmgr, action=alldebridAcct)<br>


### Authorize:

RunScript(script.module.acctmgr, action=traktAuth)<br>
RunScript(script.module.acctmgr, action=mdblistAuth)<br>
RunScript(script.module.acctmgr, action=realdebridAuth)<br>
RunScript(script.module.acctmgr, action=premiumizeAuth)<br>
RunScript(script.module.acctmgr, action=alldebridAuth)<br>
RunScript(script.module.acctmgr, action=torboxAuth)<br>
RunScript(script.module.acctmgr, action=offcloudAuth)<br>
RunScript(script.module.acctmgr, action=easynewsAuth)<br>


### ReSync:

RunScript(script.module.acctmgr, action=traktReSync)<br>
RunScript(script.module.acctmgr, action=mdblistReSync)<br>
RunScript(script.module.acctmgr, action=realdebridReSync)<br>
RunScript(script.module.acctmgr, action=premiumizeReSync)<br>
RunScript(script.module.acctmgr, action=alldebridReSync)<br>
RunScript(script.module.acctmgr, action=torboxReSync)<br>
RunScript(script.module.acctmgr, action=offcloudReSync)<br>
RunScript(script.module.acctmgr, action=easynewsReSync)<br>


### Revoke Service:

RunScript(script.module.acctmgr, action=traktRevoke)<br>
RunScript(script.module.acctmgr, action=mdblistRevoke)<br>
RunScript(script.module.acctmgr, action=realdebridRevoke)<br>
RunScript(script.module.acctmgr, action=premiumizeRevoke)<br>
RunScript(script.module.acctmgr, action=alldebridRevoke)<br>
RunScript(script.module.acctmgr, action=torboxRevoke)<br>
RunScript(script.module.acctmgr, action=offcloudRevoke)<br>
RunScript(script.module.acctmgr, action=easynewsRevoke)<br>


### Revoke All Services & Add-ons

RunScript(script.module.acctmgr, action=allRevoke)<br>


### View Authorizations:

RunScript(script.module.acctmgr, action=traktViewer)<br>
RunScript(script.module.acctmgr, action=mdblistViewer)<br>
RunScript(script.module.acctmgr, action=realdebridViewer)<br>
RunScript(script.module.acctmgr, action=premiumizeViewer)<br>
RunScript(script.module.acctmgr, action=alldebridViewer)<br>
RunScript(script.module.acctmgr, action=torboxViewer)<br>
RunScript(script.module.acctmgr, action=offcloudViewer)
RunScript(script.module.acctmgr, action=easynewsViewer)<br>


# Tools:

### Set Max Resolution:

RunScript(script.module.acctmgr, action=setUHD)<br>
RunScript(script.module.acctmgr, action=setHD)<br>
RunScript(script.module.acctmgr, action=setSD)<br>


### Set Source Select/Autoplay:

RunScript(script.module.acctmgr, action=setDIR)<br>
RunScript(script.module.acctmgr, action=setAUTO)<br>


### Install/Uninstall TMdB Helper Players:

RunScript(script.module.acctmgr, action=setPLAYER)<br>
RunScript(script.module.acctmgr, action=delPLAYER)<br>
