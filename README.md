
### Administration  
Command and aliases | Description | Usage
----------------|--------------|-------
`.greet`  |  Enables or Disables anouncements on the current channel when someone joins the server.
`.greetmsg`  |  Sets a new announce message. Type %user% if you want to mention the new member. |  .greetmsg Welcome to the server, %user%.
`.bye`  |  Enables or Disables anouncements on the current channel when someone leaves the server.
`.byemsg`  |  Sets a new announce leave message. Type %user% if you want to mention the new member. |  .byemsg %user% has left the server.
`.byepm`  |  Toggles whether the good bye messages will be sent in a PM or in the text channel.
`.greetpm`  |  Toggles whether the greet messages will be sent in a PM or in the text channel.
`.logserver`  |  Toggles logging in this channel. Logs every message sent/deleted/edited on the server. BOT OWNER ONLY. SERVER OWNER ONLY.
`.userpresence`  |  Starts logging to this channel when someone from the server goes online/offline/idle. BOT OWNER ONLY. SERVER OWNER ONLY.
`.voicepresence`  |  Toggles logging to this channel whenever someone joins or leaves a voice channel you are in right now. BOT OWNER ONLY. SERVER OWNER ONLY.
`.rotateplaying`, `.ropl`  |  Toggles rotation of playing status of the dynamic strings you specified earlier.
`.addplaying`, `.adpl`  |  Adds a specified string to the list of playing strings to rotate. Supported placeholders: %servers%, %users%, %playing%, %queued%, %trivia%
`.listplaying`, `.lipl`  |  Lists all playing statuses with their corresponding number.
`.removeplaying`, `.repl`, `.rmpl`  |  Removes a playing string on a given number.
`.sr`, `.setrole`  |  Sets a role for a given user. |  .sr @User Guest
`.rr`, `.removerole`  |  Removes a role from a given user. |  .rr @User Admin
`.r`, `.role`, `.cr`  |  Creates a role with a given name. |  .r Awesome Role
`.rolecolor`, `.rc`  |  Set a role's color to the hex or 0-255 rgb color value provided. |  .color Admin 255 200 100 or .color Admin ffba55
`.roles`  |  List all roles on this server or a single user if specified.
`.b`, `.ban`  |  Bans a mentioned user.
`.k`, `.kick`  |  Kicks a mentioned user.
`.mute`  |  Mutes mentioned user or users.
`.unmute`  |  Unmutes mentioned user or users.
`.deafen`, `.deaf`  |  Deafens mentioned user or users
`.undeafen`, `.undeaf`  |  Undeafens mentioned user or users
`.rvch`  |  Removes a voice channel with a given name.
`.vch`, `.cvch`  |  Creates a new voice channel with a given name.
`.rch`, `.rtch`  |  Removes a text channel with a given name.
`.ch`, `.tch`  |  Creates a new text channel with a given name.
`.st`, `.settopic`  |  Sets a topic on the current channel.
`.uid`, `.userid`  |  Shows user ID.
`.cid`, `.channelid`  |  Shows current channel ID.
`.sid`, `.serverid`  |  Shows current server ID.
`.stats`  |  Shows some basic stats for Bot.
`.heap`  |  Shows allocated memory - OWNER ONLY
`.prune`  |  Prunes a number of messages from the current channel. |  .prune 5
`.die`, `.graceful`  |  Works only for the owner. Shuts the bot down and notifies users about the restart.
`.clr`  |  Clears some of Bot's (or some other user's if supplied) messages from the current channel. |  .clr @X
`.newname`, `.setname`  |  Give the bot a new name.
`.newavatar`, `.setavatar`  |  Sets a new avatar image for the Bot.
`.setgame`  |  Sets the bots game.
`.checkmyperms`  |  Checks your userspecific permissions on this channel.
`.commsuser`  |  Sets a user for through-bot communication. Only works if server is set. Resets commschannel.**Owner only**.
`.commsserver`  |  Sets a server for through-bot communication.**Owner only**.
`.commschannel`  |  Sets a channel for through-bot communication. Only works if server is set. Resets commsuser.**Owner only**.
`.send`  |  Send a message to someone on a different server through the bot.**Owner only.**
  |  .send Message text multi word!
`.menrole`, `.mentionrole`  |  Mentions every person from the provided role or roles (separated by a ',') on this server. Requires you to have mention everyone permission.
`.parsetosql`  |  Loads exported parsedata from /data/parsedata/ into sqlite database.
`.unstuck`  |  Clears the message queue. **OWNER ONLY**
`.donators`  |  List of lovely people who donated to keep this project alive.
`.adddon`, `.donadd`  |  Add a donator to the database.
`.videocall`  |  Creates a private appear.in video call link for you and other mentioned people. The link is sent to mentioned people via a private message.

### Help  
Command and aliases | Description | Usage
----------------|--------------|-------
`-h`, `-help`, `@BotName help`, `@BotName h`, `~h`  |  Either shows a help for a single command, or PMs you help link if no arguments are specified. |  '-h !m q' or just '-h' 
`-hgit`  |  OWNER ONLY commandlist.md file generation.
`-readme`, `-guide`  |  Sends a readme and a guide links to the channel.
`-donate`, `~donate`  |  Instructions for helping the project!
`.modules`, `-modules`  |  List all bot modules.
`.commands`, `-commands`  |  List all of the bot's commands from a certain module.

### Permissions  
Command and aliases | Description | Usage
----------------|--------------|-------
`;permrole`, `;pr`  |  Sets a role which can change permissions. Or supply no parameters to find out the current one. Default one is 'Bot'.
`;verbose`, `;v`  |  Sets whether to show when a command/module is blocked. |  ;verbose true
`;serverperms`, `;sp`  |  Shows banned permissions for this server.
`;roleperms`, `;rp`  |  Shows banned permissions for a certain role. No argument means for everyone. |  ;rp AwesomeRole
`;channelperms`, `;cp`  |  Shows banned permissions for a certain channel. No argument means for this channel. |  ;cp #dev
`;userperms`, `;up`  |  Shows banned permissions for a certain user. No argument means for yourself. |  ;up Kwoth
`;sm`, `;servermodule`  |  Sets a module's permission at the server level. |  ;sm [module_name] enable
`;sc`, `;servercommand`  |  Sets a command's permission at the server level. |  ;sc [command_name] disable
`;rm`, `;rolemodule`  |  Sets a module's permission at the role level. |  ;rm [module_name] enable [role_name]
`;rc`, `;rolecommand`  |  Sets a command's permission at the role level. |  ;rc [command_name] disable [role_name]
`;cm`, `;channelmodule`  |  Sets a module's permission at the channel level. |  ;cm [module_name] enable [channel_name]
`;cc`, `;channelcommand`  |  Sets a command's permission at the channel level. |  ;cc [command_name] enable [channel_name]
`;um`, `;usermodule`  |  Sets a module's permission at the user level. |  ;um [module_name] enable [user_name]
`;uc`, `;usercommand`  |  Sets a command's permission at the user level. |  ;uc [command_name] enable [user_name]
`;asm`, `;allservermodules`  |  Sets permissions for all modules at the server level. |  ;asm [enable/disable]
`;asc`, `;allservercommands`  |  Sets permissions for all commands from a certain module at the server level. |  ;asc [module_name] [enable/disable]
`;acm`, `;allchannelmodules`  |  Sets permissions for all modules at the channel level. |  ;acm [enable/disable] [channel_name]
`;acc`, `;allchannelcommands`  |  Sets permissions for all commands from a certain module at the channel level. |  ;acc [module_name] [enable/disable] [channel_name]
`;arm`, `;allrolemodules`  |  Sets permissions for all modules at the role level. |  ;arm [enable/disable] [role_name]
`;arc`, `;allrolecommands`  |  Sets permissions for all commands from a certain module at the role level. |  ;arc [module_name] [enable/disable] [channel_name]
`;ubl`  |  Blacklists a mentioned user. |  ;ubl [user_mention]
`;ucl`  |  Blacklists a mentioned channel (#general for example). |  ;ubl [channel_mention]
`;usl`  |  Blacklists a server by a name or id (#general for example). |  ;usl [servername/serverid]

### Conversations  
Command and aliases | Description | Usage
----------------|--------------|-------
`\o\`  |  Bot replies with /o/
`/o/`  |  Bot replies with \o\
`..`  |  Adds a new quote with the specified name (single word) and message (no limit). |  .. abc My message
`...`  |  Shows a random quote with a specified name. |  .. abc
`@BotName copyme`, `@BotName cm`  |  Bot starts copying everything you say. Disable with cs
`@BotName cs`, `@BotName copystop`  |  Bot stops copying you
`@BotName req`, `@BotName request`  |  Requests a feature for Bot. |  @Bot req new_feature
`@BotName lr`  |  PMs the user all current Bot requests.
`@BotName dr`  |  Deletes a request. Only owner is able to do this.
`@BotName rr`  |  Resolves a request. Only owner is able to do this.
`@BotName uptime`  |  Shows how long Bot has been running for.
`@BotName die`  |  Works only for the owner. Shuts the bot down.
`@BotName do you love me`  |  Replies with positive answer only to the bot owner.
`@BotName how are you`  |  Replies positive only if bot owner is online.
`@BotName insult`  |  Insults @X person. |  @Bot insult @X.
`@BotName praise`  |  Praises @X person. |  @Bot praise @X.
`@BotName pat`  |  Pat someone ^_^
`@BotName cry`  |  Tell Bot to cry. You are a heartless monster if you use this command.
`@BotName are you real`  |  Useless.
`@BotName are you there`, `@BotName !`, `@BotName ?`  |  Checks if Bot is operational.
`@BotName draw`  |  Bot instructs you to type $draw. Gambling functions start with $
`@BotName fire`  |  Shows a unicode fire message. Optional parameter [x] tells her how many times to repeat the fire. |  @Bot fire [x]
`@BotName rip`  |  Shows a grave image of someone with a start year |  @Bot rip @Someone 2000
`@BotName j`  |  Joins a server using a code.
`@BotName slm`  |  Shows the message where you were last mentioned in this channel (checks last 10k messages)
`@BotName bb`  |  Says bye to someone.  |  @Bot bb @X
`@BotName call`  |  Useless. Writes calling @X to chat. |  @Bot call @X 
`@BotName hide`  |  Hides Bot in plain sight!11!!
`@BotName unhide`  |  Unhides Bot in plain sight!1!!1
`@BotName dump`  |  Dumps all of the invites it can to dump.txt.** Owner Only.**
`@BotName ab`  |  Try to get 'abalabahaha'
`@BotName av`, `@BotName avatar`  |  Shows a mentioned person's avatar.  |  ~av @X

### Gambling  
Command and aliases | Description | Usage
----------------|--------------|-------
`$draw`  |  Draws a card from the deck.If you supply number [x], she draws up to 5 cards from the deck. |  $draw [x]
`$shuffle`, `$reshuffle`  |  Reshuffles all cards back into the deck.
`$flip`  |  Flips coin(s) - heads or tails, and shows an image. |  `$flip` or `$flip 3`
`$roll`  |  Rolls 2 dice from 0-10. If you supply a number [x] it rolls up to 30 normal dice. |  $roll [x]
`$nroll`  |  Rolls in a given range. |  `$nroll 5` (rolls 0-5) or `$nroll 5-15`
`$raffle`  |  Prints a name and ID of a random user from the online list from the (optional) role.
`$$$`  |  Check how many BotFlowers you have.

### Games  
Command and aliases | Description | Usage
----------------|--------------|-------
`t`, `-t`  |  Starts a game of trivia.
`tl`, `-tl`, `tlb`, `-tlb`  |  Shows a current trivia leaderboard.
`tq`, `-tq`  |  Quits current trivia after current question.
`typestart`  |  Starts a typing contest.
`typestop`  |  Stops a typing contest on the current channel.
`typeadd`  |  Adds a new article to the typing contest. Owner only.
`>poll`  |  Creates a poll, only person who has manage server permission can do it. |  >poll Question?;Answer1;Answ 2;A_3
`>pollend`  |  Stops active poll on this server and prints the results in this channel.
`,createwar`, `,cw`  |  Creates a new war by specifying a size (>10 and multiple of 5) and enemy clan name. | ,cw 15 The Enemy Clan
`,sw`, `,startwar`  |  Starts a war with a given number.
`,listwar`, `,lw`  |  Shows the active war claims by a number. Shows all wars in a short way if no number is specified. |  ,lw [war_number] or ,lw
`,claim`, `,call`, `,c`  |  Claims a certain base from a certain war. You can supply a name in the third optional argument to claim in someone else's place.  |  ,call [war_number] [base_number] (optional_otheruser)
`,cf`, `,claimfinish`  |  Finish your claim if you destroyed a base. Optional second argument finishes for someone else. |  ,cf [war_number] (optional_other_name)
`,unclaim`, `,uncall`, `,uc`  |  Removes your claim from a certain war. Optional second argument denotes a person in whos place to unclaim |  ,uc [war_number] (optional_other_name)
`,endwar`, `,ew`  |  Ends the war with a given index. | ,ew [war_number]
`>choose`  |  Chooses a thing from a list of things |  >choose Get up;Sleep;Sleep more
`>8ball`  |  Ask the 8ball a yes/no question.
`>`  |  Attack a person. Supported attacks: 'splash', 'strike', 'burn', 'surge'. |  > strike @User
`poketype`  |  Gets the users element type. Use this to do more damage with strike!

### Music  
Command and aliases | Description | Usage
----------------|--------------|-------
`!m n`, `!m next`  |  Goes to the next song in the queue.
`!m s`, `!m stop`  |  Stops the music and clears the playlist. Stays in the channel.
`!m d`, `!m destroy`  |  Completely stops the music and unbinds the bot from the channel. (may cause weird behaviour)
`!m p`, `!m pause`  |  Pauses or Unpauses the song.
`!m q`, `!m yq`  |  Queue a song using keywords or a link. Bot will join your voice channel. **You must be in a voice channel**. |  `!m q Dream Of Venice`
`!m lq`, `!m ls`, `!m lp`  |  Lists up to 15 currently queued songs.
`!m np`, `!m playing`  |  Shows the song currently playing.
`!m vol`  |  Sets the music volume 0-150%
`!m dv`, `!m defvol`  |  Sets the default music volume when music playback is started (0-100). Does not persist through restarts. |  !m dv 80
`!m min`, `!m mute`  |  Sets the music volume to 0%
`!m max`  |  Sets the music volume to 100% (real max is actually 150%).
`!m half`  |  Sets the music volume to 50%.
`!m sh`  |  Shuffles the current playlist.
`!m setgame`  |  Sets the game of the bot to the number of songs playing.**Owner only**
`!m pl`  |  Queues up to 25 songs from a youtube playlist specified by a link, or keywords.
`!m lopl`  |  Queues up to 50 songs from a directory.
`!m radio`, `!m ra`  |  Queues a direct radio stream from a link.
`!m lo`  |  Queues a local file by specifying a full path. BOT OWNER ONLY.
`!m mv`  |  Moves the bot to your voice channel. (works only if music is already playing)
`!m rm`  |  Remove a song by its # in the queue, or 'all' to remove whole queue.

### Searches  
Command and aliases | Description | Usage
----------------|--------------|-------
`~lolchamp`  |  Shows League Of Legends champion statistics. If there are spaces/apostrophes or in the name - omit them. Optional second parameter is a role. | ~lolchamp Riven or ~lolchamp Annie sup
`~lolban`  |  Shows top 6 banned champions ordered by ban rate. Ban these champions and you will be Plat 5 in no time.
`~yt`  |  Searches youtubes and shows the first result
`~ani`, `~anime`, `~aq`  |  Queries anilist for an anime and shows the first result.
`~mang`, `~manga`, `~mq`  |  Queries anilist for a manga and shows the first result.
`~randomcat`  |  Shows a random cat image.
`~i`  |  Pulls the first image found using a search parameter. Use ~ir for different results. |  ~i cute kitten
`~ir`  |  Pulls a random image using a search parameter. |  ~ir cute kitten
`lmgtfy`, `~lmgtfy`  |  Google something for an idiot.
`~hs`  |  Searches for a Hearthstone card and shows its image. Takes a while to complete. | ~hs Ysera
`~osu`  |  Shows osu stats for a player. | ~osu Name
`~ud`  |  Searches Urban Dictionary for a word. | ~ud Pineapple
`~#`  |  Searches Tagdef.com for a hashtag. | ~# ff

### NSFW  
Command and aliases | Description | Usage
----------------|--------------|-------
`~hentai`  |  Shows a random NSFW hentai image from gelbooru and danbooru with a given tag. Tag is optional but preffered. (multiple tags are appended with +) |  ~hentai yuri+kissing
`~danbooru`  |  Shows a random hentai image from danbooru with a given tag. Tag is optional but preffered. (multiple tags are appended with +) |  ~danbooru yuri+kissing
`~gelbooru`  |  Shows a random hentai image from gelbooru with a given tag. Tag is optional but preffered. (multiple tags are appended with +) |  ~gelbooru yuri+kissing
`~e621`  |  Shows a random hentai image from e621.net with a given tag. Tag is optional but preffered. Use spaces for multiple tags. |  ~e621 yuri+kissing
`~cp`  |  We all know where this will lead you to.
`~boobs`  |  Real adult content.
`~butts`, `~ass`, `~butt`  |  Real adult content.
na
