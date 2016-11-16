## Skype Integration
#### Installation
The easiest way to install this integration is to use KPM.
```sh
/kpm install skype
```

#### Configuration
To add a configuration, execute each of the following commands (replace each of the angle bracketed strings with the respective information):
```sh
/kpm config skype username "<skypeUsername/skypeEmail>"
/kpm config skype password "<skypePassword>"
/kpm config skype acceptContactRequests true
/kpm config skype conversations ["<conversationID1>","<conversationID2",...]
/kpm config skype commandPrefix "!"
```

|Property|Explanation|
|-|-|
|`username`|Username of the bot account.|
|`password`|Password of the bot account.|
|`commandPrefix`|Command prefix to use with the bot. Note: skype reserves the '/' prefix for its own special commands.|
|`acceptContactRequests`|Optional (default=true). Wheather contact requests to the bot should be automatically accepted.|
|`conversations`|Optional (default=any). ID's of conversations to listen to.|

#### Running
To run Skype, either run `node main.js skype` when starting Concierge or run `/kpm start skype` when Concierge is running.
