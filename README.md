# Discord-Gambling-Bot
This is a gambling discord bot. You can have fun at the roulette table without any real risk. Bring your discord together by competing with your friends.

# Commands

All commands by default begin with "$" and some end in "%". These can be changed in the GambaBot.java class.

# Standard Commands
- "$accept" - Allows the user to accept a duel that was issued by another user.
- "$balance" - Allows the user to check their balance.
- "$commands" - Allows the user to check the commands in discord.
- "$create profile" - Users may only start gambling when they create a profile.
- "$current rank" - Displays current rank of user.
- "$duel (@name) (amount)" - The user issues a duel with another player. Winner gets duel amount from loser.
- "$give (@name) (amount)" - The user gives another user stated amount of money.
- "$leaderboard" - Displays the top five users and their balances.
- "$roulette (amount)" - The user gambles on a 50/50 chance to double stated amount.
- "$roulette% (1-100)" - The user wagers a percentage of their balance rounded to the nearest whole number in a 50/50 chance.

# Admin Commands
- "$add (@user) (amount)" - Adds stated amount to stated user's balance.
- "$promote (@user)" - Stated user may now use admin commands.
- "$raffle (amount (1-10000))" - Starts a raffle to win stated amount for free just by reacting to raffle message.
- "$remove (@user) (amount)" - Removes stated amount from stated user's balance.
- "$set (@user) (amount)" - Sets stated user's balance to stated amount.

# Side Notes
- Any command requiring an "(amount)" requires a whole number.
- If the user running the bot adds an instance of it to multiple servers, it may share the same data structure with the other servers.
    - Users may see names they don't recognize from their server when checking the leaderboard.
- The bot will create a json file to save, update, and load user profiles where the bot is being run.
    - The json file is editable by the one running the code, be careful however because if you mess up the formatting, it may throw an error trying to load,              update, or save profiles. So it is highly advised against.
    - The bot will save profiles every hour. In case bot is down, just run the code again and it should reload all user profiles.
    - Profiles are saved in order of balance from highest to lowest.
- This code is free to use, just please don't try to pass it off as your own. That will make me sad.
    - It is advised that you have at least some programming knowledge before trying to change the code. That doesn't mean you can't try though.
    - With the code being free to use, that means you may modify/improve it on your own.
    - Changing anything about the User objects may result in you needing to update how the program saves, updates, and loads profiles. It was made specifically for       how the object class is set up.
- This program is not perfect, there may be bugs still around I did not find myself.
