# Azure Pipeline Linux agent

Easy to use docker image for creating a self-hosted Azure Pipeline Linux agent.

Changelog

- March 22:
  - reworked the dockerfile structure
  - added git to the agent
  - added --replace to override any existing agent with same name
  - added Azure CLI
  - added Powershell 7.1.3
  - added sqlpackage
  - changed base image from debian to ubuntu 18.04
  - added logging output
  - used some code from official MS documentation about running self-hosted Linux agents in docker
- March 19: Update
- February 2021: Created

```console
docker run -e ORGANIZATION=myorganization 
           -e PAT=your_personal_access_token_very_long_hash 
           -e AGENT=agent_name 
           -e POOL=agent_pool_name czmirek/azure-pipeline-linux-agent:latest
```
