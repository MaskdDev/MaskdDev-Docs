# WriterStats Changelog - All Updates

## Version 2.7.0

- Added /choose to allow you to pick between two options. (Early Access)
- Added /flip and /roll to flip a coin and roll a dice. (Early Access)
- Added /define to fetch the definition for any English word. (Early Access)
- Added /generate to help you generate names for your next project! (Early Access)

### Added

- `/choose`
- `/flip`
- `/roll`
- `/define`
- `/generate`

## Version 2.6.0

- Added /importdata writerbot to import your data from Writer-bot!

### Added

- `/importdata writerbot`

## Patch 2.5.1

- /session group now checks for permissions in specific channel before starting to prevent errors.
- Custom dynamic status support has been added to show number of servers and number of users in WriterStats' status.
- Updated update pending message for creating new sessions to include prompt to join support server and to try again later.

### Modified

- `/session group`
- `/session individual`

## Version 2.5.0

- Added /secrets, a patron-only command to view hidden WriterStats features!
- Added infrastructure to store the server of each session. This is in preparation for future server-related commands.
- Added /day statistics commands to view statistics for a specified day.
- Added /project day statistics commands to view statistics for a project for a specified day.
- Created the "Patrons" category for patron-only commands!
- /between is no longer project-specific.
- Modified profile user command to show up as "View Writer Profile" in the apps menu.
- /week and /project week now accept the standard date options.
- Added /discord to get a link to the support server.
- Added /ping to view the bot's response latency.
- Updated /support to display the latest patron benefits.

### Added

- `/secrets`
- `/day today`
- `/day yesterday`
- `/day find`
- `/project day today`
- `/project day yesterday`
- `/project day find`
- `/discord`
- `/ping`

### Modified

- `/between`
- `/support`
- `/week find`
- `/project week find`

## Patch 2.4.1

- Session start embeds now display the correct starting wordcount if both a project and starting wordcount have been set.

### Modified

- `/session join`
- `/session group`
- `/session individual`

## Version 2.4.0

- You can now run sessions without an active project!
- You can now specify an alternate starting wordcount when creating/joining a session. This overrides your current project wordcount for calculating the net change, but doesn't directly affect it.
- /week and /month commands now display user statistics instead of statistics for your current project.
- /project week and /project month have been added, allowing you to see the statistics for your active project.
- Project names now have a maximum length of 50 characters.
- You can now delete past sessions with /session delete and edit them with /session edit!
- You can now view details of a past session with /session view.
- /quickstart and /guide have been modified to be up to date with the new project system.
- Updated MaskdDev Docs to reflect the new changes.
- /help now has a slightly modified format to accomodate the new commands and subcommand groups.

### Added

- `/project week`
- `/project month`
- `/project none`
- `/session edit`
- `/session delete`
- `/session view`

### Modified

- `/session group`
- `/session individual`
- `/session join`
- `/week`
- `/month`
- `/quickstart`
- `/guide`
- `/help`

## Patch 2.3.2

- WriterStats prevents you from starting a group session without the bot having the appropriate permissions.

### Modified

- `/session group`

## Patch 2.3.1

- Fixed poor wording in session start embed.
- /session manual now accepts minutes by default and has a variety of other options for the date and time fields.

### Modified

- `/session group`
- `/session manual`

## Version 2.3.0

- Two new options for random times: Medium and Chaos! The mininum length of a long random session has switched from 20 minutes to 40 minutes.
- Group session leaderboards now display spectators and people who didn't submit a wordcount.
- Group session leaderboards are now sent once the final member has submitted their wordcount.
- Group session leaderboards ALSO now display the top 10, including people who didn't submit a wordcount!
- Guide embed now displaying embed 5.
- /support now displays perks of becoming a member!
- Changelog now uses "-" instead of "#" to prepare for markdown.

### Modified

- `/session individual`
- `/session group`
- `/support`
- `/changelog`
- `/guide`

## Patch 2.2.2

- New stats option: Number of Users
- Added backend tools to safely push updates without interrupting sessions.

### Modified

- `/bot stats`

## Patch 2.2.1

- /goals history is now working.
- /session individual and /session group no longer send messages twice, under very specific circumstances.
- Changelog for 2.2.0 now included in changelog.

### Modified

- `/help`
- `/session group`

## Version 2.2.0

- Group sessions now have a configurable wait time for results.
- Projects can now be renamed using the `/project rename` command.
- Bot Invite Link removed from `/help` and replaced with the documentation link.

### Added

- `/project rename`

### Modified

- `/help`
- `/session group`

## Version 2.1.0

- Group session embeds only update BEFORE the session has started.
- Patrons are now distinguishable in WriterStats.
- Patrons now have a purple profile colour, with a tag showing how long they've been supporting WriterStats!
- /between: Patron-only command to get your writing stats between any two dates.

### Added

- `/between`

## Patch 2.0.1

- Fixed /settimezone showing 12:XX AM instead of 12:XX PM when setting a timezone.
- /session manual no longer updates your project wordcount.
- Maintenance mode has been added to stop the creation of new sessions and allow current users to finish their sessions before an update.

### Modified

- `/settimezone`
- `/session individual`
- `/session group`
- `/session manual`

## Version 2.0.0

- Added a lot of commands, shown in the field below.
- Renamed commands to be consistent with the new version 2.0 scheme.

### Added

- `/guide`
- `/leaderboard`
- `/preferences view`
- `/preferences toggle`
- `/profile`
- `/quickstart`
- `/project setcount`
- `/project setgoal`
- `/project info`
- `/session individual`
- `/session group`
- `/session join`
- `/session spectate`
- `/session leave`
- `/session info`
- `/goals set`
- `/goals remove`
- `/goals view`
- `/goals history`
- `/channel stats`
- `/month current`
- `/month last`
- `/month find`
- `/week current`
- `/week last`
- `/week find`

### Modified

- `/help`
- `/support`
- `/session complete`
- `/session cancel`
- `/session manual`

### Removed

- `/thisweek`
- `/lastweek`
- `/session start`

## Version 1.3.0

- Renamed /stats and /changelog to /bot stats and /bot changelog to avoid confusion with other commands.
- Fixed bug where commands weren't showing up to non-moderators.
- Added a prompt to remind users to use the DD/MM/YYYY format in /session manual, if date is entered incorrectly.

### Added

- `/bot stats`
- `/bot changelog`

### Modified

- `/session manual`

### Removed

- `/stats`
- `/changelog`

## Version 1.2.0

- Added the /support command to allow users to support the bot and its development.

### Added

- `/support`

## Patch 1.1.1

- Patched bot not responding when creating a new session in a new week.
- Fixed error handling for /session manual

## Version 1.1.0

- Added option to load previous sessions into a project!
- Improved readability and UI of statistics menus.

### Added

- `/session manual`

### Modified

- `/thisweek`
- `/lastweek`

## Version 1.0.0

- Added base functionality. See added commands for more info.

### Added

- `/help`
- `/changelog`
- `/stats`
- `/settimezone`
- `/project new`
- `/project setactive`
- `/project delete`
- `/session start`
- `/session cancel`
- `/session complete`
- `/lastweek`
- `/thisweek`
