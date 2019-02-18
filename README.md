# MacOS LaunchAgents/LaunchDaemons

## LaunchAgents
Launch Agents & Daemons run as specific users, after they have logged in.

In order for Launch Agents to function properly, place them in `~/Library/LaunchAgents`.

Run the following commands to enable/disable specific configurations:

- Enable - `launchctl load -w ~/Library/LaunchAgents/FILENAME.plist`
- Disable - `launchctl unload -w ~/Library/LaunchAgents/FILENAME.plist`

## LaunchDaemons
Launch Daemons run while the system is booted. No user login required.

In order for Launch Daemons to function properly, place them in `/Library/LaunchDaemons`.

Run the following commands to enable/disable specific configurations:

- Enable: `launchctl load -w /Library/LaunchDaemons/FILENAME.plist`
- Disable: `launchctl unload -w /Library/LaunchDaemons/FILENAME.plist`


# Contributors

* Aaron Fagan - [Github](https://github.com/aaronfagan), [Website](https://www.aaronfagan.ca/)