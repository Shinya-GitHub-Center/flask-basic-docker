# Basic starter for the study of Flask Development

## Requirement
- Any Linux Distribution (I have not tested with WSL on Windows...)
- docker
- docker compose
- Your favorite CUI Terminal / Your favorite VSCode

## Get Started!!
1. Download the souce code via zip and unzip it  
(I don't recommend `git clone` this repository, since you possibly would make your own flask project git-lize later, this might occur some conflict with upper git directory)
2. On your terminal, move to the root directory (where `docker-compose.yml` exsists)
3. Run the following commands
```
$ docker compose up -d
$ docker exec -it <container name> bash
$ poetry new <desired project name> --name app
$ cd <desired project name>
```
