# Custom GitHub Actions

Setting up JavaScript Action
cd employee-js-action
Run the following commands
 - npm init -y
 - npm install @actions/core actions/github @slack/web-api


Setting up Docker Action
cd employee-docker-action
- dotnet new console -o src -n DotNetDockerAction
- cd src
- dotnet add package Octokit
- dotnet add package Slack.NetStandard

