# unityItchTest
### Required secrets: 
#### Unity:

Since unity require a valid unity license and login information, I would probably create a new unity account for this. These variables can be reused for multiple projects. If you have a enterprise unity license then you should be able to use an API key to login instead.

`UNITY_LICENSE`

This secret should contain the full contents of your unity license file. You should be able to find it here: 

Windows: `C:\ProgramData\Unity\Unity_lic.ulf`

Mac: `/Library/Application Support/Unity/Unity_lic.ulf`

Linux: `~/.local/share/unity3d/Unity/Unity_lic.ulf`


If this file path does not exist, open unity hub, go into settings->licenses and press `Add Lisence` and add a peronal license.

`UNITY_EMAIL`

This is the email for your unity user. 

`UNITY_PASSWORD`

This is the password for your unity user.

#### Itch:

`BUTLER_API_KEY`

This is your API key. To get a key, go to the itch.io website and go to settings->api and press `Generate Api Key`.

Additionally, add these two secrets. They are not required to be secret, but are anyway.

`ITCH_USER`

Your Itch username

`ITCH_PAGE` 

The page you are pushing to. Specifically the url endpoint of the page. 

Example: If your itch page you have created has this url `https://username.itch.io/page`, put in the specified parts of the url into the last secrets.