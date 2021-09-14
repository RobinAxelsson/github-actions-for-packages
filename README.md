# Tic Tac Toe Game

Let's learn about CD while using GitHub Actions and the GitHub Package Registry!


```shell
    token robinaxelsson github-token-docker-packages | docker login docker.pkg.github.com -u robinaxelsson --password-stdin
    docker pull docker.pkg.github.com/robinaxelsson/github-actions-for-packages/tic-tac-toe:sha-9994332
    id=$(docker images -q | sed -n '1p')
    docker run -d -it --rm -p 8080:80 --name ttt $id
```
Open localhost:8080
Play tic-tac-toe
```shell
    docker ps
    docker stop <id>
    docker rm <id>

NOTE: Tutorial is close to obsolete with a lot of warnings about newer code.

