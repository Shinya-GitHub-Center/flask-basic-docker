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
$ poetry shell
$ poetry add flask
```

## To finish today's your flask development (With enjoyable 3 exits!!)
1. `exit` => Exit virtualenv
2. `exit` => Exit docker container (going back to host)
3. `docker compose down` => Remove docker container
4. `exit` => Close your terminal

## To resume yesterday's your flask development
Run the following commands @ where docker-compose.yml exsists
```
$ docker compose up -d
$ docker exec -it <container name> bash
$ cd <your project name>
$ poetry shell
```
