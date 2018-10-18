# FantasyAggregator
Fantasy Football App to easily manage multiple Fantasy Football Teams.  Initially this will only be for Yahoo NFL Fantasy, with the hope to expand to other sports and sites as I get more comfortable with how to manage API's.  On that note Yahoo's API documentation is pretty bad so I will try my best to document any discoveries I make in this respository.

## API Keys ##
The API Keys are hidden using the method below

https://gist.github.com/derzorngottes/3b57edc1f996dddcab25

## Recreating Config.js ##
Follow the instructions above to recreate the config.js in the root directory each applications API Keys are stored in the following manner:

### Yahoo API ###

```javascript 
var YAHOO_API = {
  AppID : '123456',
  ClientID : '56789',
  ClientSecret : '101010'
}
```



## YAHOO API NOTES ##
To get a users nfl teams in JSON (to get XML drop "?format=json":

`
https://fantasysports.yahooapis.com/fantasy/v2/users;use_login=1/games;game_keys=nfl/teams?format=json
`
