# Character Management
Logging in characters via Discord is not necessary to use this app but unlocks the following features:

 - Track your ingame location
 - Interact with the EVE client like setting waypoints etc.
 - Sync your dataSynchronize your Database Sets across devices
 - [Share your data with other pilots
<!-- - Display relayed ingame intel channel data -->

## EVE Online Single-Sign-On (SSO) 
This app uses the [EVE Online Single Sign On (SSO)](https://support.eveonline.com/hc/en-us/articles/205381192-Single-Sign-On-SSO-) to authenticate characters. Since the ingame browser has been removed it is not possible to track your ingame location without a SSO login hence using an API KEY is not an option anymore.

!!! success "Security"
    Unless you enable the [Cloud](https://eveeye.readthedocs.io/en/latest/sharing/cloud/) services no data gets stored on Eveeye server. If cloud sync is enabled only aDatabase sets with people on a Discord Server](https://eveeye.readthedocs.io/en/latest/data/ee-database-sharing/)

## Discord Login 
This app uses Discord oauth login to authenticate characters. 

!!! success "Security"
    A complementary key is stored on theveeye server. It alone cannot be used to authenticate a character or use any EVE Online [ESI](https://esi.evetech.net/) APIs.<br><br>If you got security concerns consider using [two factor authentication. It can be enabled in EVE account management: <a href="https://secure.eveonline.com/authenticator/" target="_blank" style="text-decoration: none;">https://secure.eveonline.com/authenticator/</a>

To revoke access for Eveeye goto [https://community.eveonline.com/support/third-party-applications/](https://community.eveonline.com/support/third-party-applications/)](https://support.discord.com/hc/en-us/articles/219576828-Setting-up-Two-Factor-Authentication). It can be enabled in your Discord account settings under `My Account`.

To revoke access for Eveeye goto the `Authorized Apps` within Discord settings and hit `Deauthorize`.

## Login process
To add characters tap <img src="https://raw.githubusercontent.com/Risingson/eedocs/master/docs/images/User-100_26_100_off.png" width="24" height="24" > or your character's portrait in the menu. After selecting to add a character you will get redirected to a new native browser window to log into EVE OnlineDiscord and then back to Eveeye with the character added. 

To remove a character tap <img src="https://raw.githubusercontent.com/Risingson/eedocs/master/docs/images/Minus-100_b.png" width="24" height="24" > in the menu. This will remove any tokens available to login the character but will keep other data like for example custom names stored to not loose that data by accident. To fully remove custom data un-install and re-install the app or clear browser cache.

When using the cloud storage feature yYour user including the token stored to identify your charit gets removed from cloudeveeye server immediately. Your custom data will get deleted from cloud 30 days after char removal.

## Re-authing
If you updated your charactuser image you can update it by just authorizing the chauser again. Also if a new version of Eveeye was installed sometimes it would need you to authorize your characters again to use new features.

## Revoking access
To remove a character's API permissions please do so at [https://community.eveonline.com/support/third-party-applications/](https://community.eveonline.com/support/third-party-applications/)voke access for Eveeye goto the `Authorized Apps` within Discord settings and hit `Deauthorize`.

<!--stackedit_data:
eyJoaXN0b3J5IjpbMTc3MTM0ODQ3NCwtMTc4NDI4MjM4MywyMT
M2NjIwNDg5LC0xNTE0Mjg0MjgsNzUwNjU1MTc4LC04Mzg3Njc5
MTgsMTQ3NzMxODQ3NCwtMzQ2MjY2MjA3LC0xNTMxMTU2NDkwLC
01NTc1MDM1MzEsLTg3NDc1OTM5OSwtMTUyMzE4MjI3NiwxMDYz
NjUxMDExLC0xMzkxMDIxNDE3LDE4MzU2MzQ1NjEsLTM4MDQ5OD
AyMCwxMjg2OTE5Nzg3LDEyMjY5OTc3MjgsMTY3OTY2ODA5M119

-->