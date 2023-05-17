# WriterStats Guide - Sessions

Writing tracking is done through the use of sessions. All sessions will count towards your active project, so be sure you're in the right project before you start by using `/project info`. If you make a mistake, you can cancel a session with `/session cancel`.

## Starting a Session

There are several types of sessions that you can begin. The three commands you can use to create a session are:

- `/session individual` - This sets up a session for you to write in individually. You can set up a timer for yourself to keep you on task, or leave it open ended as you settle in for the day. The session starts as soon as you run this command.

- `/session group` - Start a session that other users can join, which will display a leaderboard at the end to see who wrote the most! Group sessions must have a time limit. The default setup of a group session is 15 mins long with a 1 minute delay, but these settings can both be changed for individual sessions. Use /session join to join the group session in your current channel.

- `/session manual` - Use this to manually enter a session that you did outside of WriterStats. Enter the date, the length of the session, and the number of words written/edited in the session. This will not affect your project's current wordcount, so you may have to also use /project setcount to update this.

## Options when starting a session

`/session individual` and `/session group` both have several options you can pass into them, detailed below:

- `session_length` - This is how long the session should last in minutes. For advanced control, you can enter the time value as h/mm/ss for a maximum session length of 2hrs. eg: 1/30/00 will run a 90min (1.5hr) session. For individual sessions, you can leave this blank to start a session without a timer.

- `random_length` - For a little challenge, or if you're not sure how long you want to write for, you can select from some presets to give you a random session length from 5 to 60 mins. Choose from "Short - 5 to 20 minutes", "Long - 20 to 60 minutes", and "Random - 5 to 60 minutes" to receive a random time!

- `start_delay` - Decide how much time until the session starts to give all your writing buddies time to join! This is a minutes value and can be a maximum of 60 minutes. This option is only available for group sessions.

- `end_delay` - Decide how much time participants will have to submit their wordcount after the session ends! This is a minutes value and can be a maximum of 30 minutes. This option is only available for group sessions.

_Note:_ If you wish to start a group session as a spectator, you may use the optional `join_type` option to do so.

## Joining a group session

The `/session join` command will add you to the list of participants in a session. Upon joining, you will get a message to tell you what the bot has recorded as your active project and its current wordcount. To change this, leave the session with `/session leave` and switch your active project before rejoining.

## Spectating a group session

If you want to join a group session without a writing project, you can use `/session spectate`. You will be notified at the start and the end of the session but will not be able to submit your final stats with `/session complete` at the end of the session.

## Finishing a Session

When you are done with a session, run `/session complete` to upload your stats for the session. You must enter either a final or change value, with an optional edited value as an extra. The `/session complete` command will immediately end an individual session, whether timed or not. For group sessions, you have two minutes to submit your count at the end. After this, a leaderboard will be displayed to compare the results of competitors!

`/session complete` has 3 options, which are listed below:

- `final` - the total wordcount of your project at the end of the session. The bot will automatically calculate the difference between this and the starting wordcount of your active project to tell you how much you added/subtracted from your total. This will automatically update the total wordcount of your active project.

- `change` - manually tell the bot how many words were added/subtracted in your project. This will automatically update the total wordcount of your active project.

- `edited` - the amount of text that you have been editing/revising during the session. Either the wordcount of the section you’ve been editing, or your best-guess at the number of words that you’ve changed. This figure will count toward your goals and leaderboard stats without affecting the total wc of your project.
