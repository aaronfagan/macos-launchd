# MacOS LaunchAgents/LaunchDaemons

## LaunchAgents
Launch Agents run as a specific users, after that user has logged in.

In order for Launch Agents to function properly, place them in `~/Library/LaunchAgents`.

Run the following commands to enable/disable specific configurations:

- Enable - `launchctl load -w ~/Library/LaunchAgents/${FILENAME}.plist`
- Disable - `launchctl unload -w ~/Library/LaunchAgents/${FILENAME}.plist`

## LaunchDaemons
Launch Daemons run as root. No user login is required.

In order for Launch Daemons to function properly, place them in `/Library/LaunchDaemons`.

Run the following commands to enable/disable specific configurations:

- Enable - `launchctl load -w /Library/LaunchDaemons/${FILENAME}.plist`
- Disable - `launchctl unload -w /Library/LaunchDaemons/${FILENAME}.plist`

## Check What Is Enabled
To check what is enabled, `grep` for the `Label` value from your configuration, like this: 
```
launchctl list | grep ${LABEL}
```

# Contributors
* Aaron Fagan - [Github](https://github.com/aaronfagan), [Website](https://www.aaronfagan.ca/)
