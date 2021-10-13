# Setup

Create a new application in the [Discord Developer Portal](https://discord.com/developers/applications)

Under the application settings, select `OAuth2` to find your `CLIENT_ID` and `CLIENT_SECRET`.

I'm currently testing on **Python 3.8.10**

`pip install Flask` 

`pip install requests-oauthlib`

# Run

Run the demo server: `OAUTH2_CLIENT_ID=88115522... OAUTH2_CLIENT_SECRET=Y33zmNuN... python app.py`

> Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)

# Scopes

Scopes requested by this app

| Scope       | Description                                                                                                                                                     |
| :---------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| identify    | allows [/users/@me](https://discord.com/developers/docs/resources/user#get-current-user) without `email`                                                        |
| email       | enables [/users/@me](https://discord.com/developers/docs/resources/user#get-current-user) to return an `email`                                                  |
| guilds      | allows [/users/@me/guilds](https://discord.com/developers/docs/resources/user#get-current-user-guilds) to return basic information about all of a user's guilds |
| connections | allows [/users/@me/connections](https://discord.com/developers/docs/resources/user#get-user-connections) to return linked third-party accounts                  |

Full Discord Scopes ( [here](https://discord.com/developers/docs/topics/oauth2#shared-resources-oauth2-scopes) )
