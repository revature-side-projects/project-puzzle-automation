# Project Puzzle Automation

This project is an automation script that will connect to the [Trello REST API](https://developer.atlassian.com/cloud/trello/rest/api-group-actions/) in order to facilitate the Revature Project Puzzle Process.

The process is, at the beginning of each week, to copy the next week's worth of required tasks to each associate (represented as a list in Trello) at the bottom. This script will need access to information such as where to find the destination trello boards and what week they are currently in.

Perhaps in the future, the automation can be expanded to have different versions of the project requirements source for each destination board.

## Required Configuration

The configuration for the script will be kept in a file called `.puzzle.config.json`, at the root directory of the project. It's structure will be similar to the provided [.puzzle.config.example.json](.puzzle.config.example.json) file.

At the minimum, this script requires a Trello AppKey and a Trello Secret Token in order to authenticate with the Trello API.