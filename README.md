# Custom GitHub Actions

## 1. Setting up JavaScript Action

### Run the following commands
```bash
  cd employee-js-action
  npm init -y
  npm install @actions/core actions/github @slack/web-api
```

## 2. Setting up Docker Action
```bash
  cd employee-docker-action
  dotnet new console -o src -n DotNetDockerAction
  cd src
  dotnet add package Octokit
  dotnet add package Slack.NetStandard
```

