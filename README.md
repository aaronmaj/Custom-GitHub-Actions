## Custom GitHub Actions

### 1. Setting up JavaScript Action

#### Run the following commands
```bash
  cd employee-js-action
  npm init -y
  npm install @actions/core actions/github @slack/web-api
```

### 2. Setting up Docker Action
```bash
  cd employee-docker-action
  dotnet new console -o src -n DotNetDockerAction
  cd src
  dotnet add package Octokit
  dotnet add package Slack.NetStandard
```
### 3. Generate Slack User OAuth Token (SLACK_TOKEN) and Bot User OAuth Token
Follow along the documentation provided here:

- https://github.com/kasunkv/slack-notification/blob/master/generate-slack-token.md

Make sure you add this scope to the User Token: 
```users:read.email``` in order to view email addresses of people in a workspace

#### Add SLACK_TOKEN in GitHub's repository settings
```Choose -> Secrets and variables ``` \
```Choose Actions -> New Repository secret```

