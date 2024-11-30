# Random Joke Updater

This repository contains a GitHub Actions workflow that fetches a random joke from an API and updates the `README.md` file every hour with the new joke. It also allows manual triggering of the workflow.

## Features

- **Automatic Joke Updates**: The workflow runs every hour to fetch a random joke and updates the `README.md` with the joke's setup and punchline.
- **Manual Trigger**: The workflow can also be manually triggered using GitHub Actions' `workflow_dispatch` feature.
- **Customizable**: You can modify the placeholders in the `README.md` file to display the joke in the format you prefer.

## How It Works

The GitHub Actions workflow is set up to run at the start of every hour, or when manually triggered, and performs the following steps:

1. **Checkout Repository**: The repository is checked out to the runner.
2. **Fetch Random Joke**: A request is made to the [Official Joke API](https://official-joke-api.appspot.com/random_joke) to fetch a random joke.
3. **Update README**: The joke's setup and punchline are inserted into the `README.md` file by replacing the placeholders `Why are pirates called pirates?` and `Because they arrr!`.
4. **Commit Changes**: The changes are committed and pushed to the repository.


## Manual Trigger

If you want to manually trigger the workflow, go to the **Actions** tab in your GitHub repository, select the **Update README with Random Joke** workflow, and click **Run workflow**.



## Joke of the Hour

**Setup**: Why are pirates called pirates?

**Punchline**: Because they arrr!


