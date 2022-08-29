## NOTE: Taken from https://hub.docker.com/_/haskell/ but I don't fully understand it yet...
# Get, build and start
```
~$ git clone --branch haskell_docker git@github.com:icasimpan/learning.git haskell_docker
~$ cd haskell_docker
~$ cp .env-sample .env
~$ docker-compose build
~$ docker-compose up -d
```

# Shell-in
```
~$ docker-compose exec haskell /bin/bash
```

# Haskell Learning Resources
* https://riptutorial.com/haskell
* https://learnxinyminutes.com/docs/haskell/
* https://www.tutorialspoint.com/haskell/index.htm

# Optional
You can use docktie if you aren't too familiar with docker in the meantime - https://github.com/docktie/docktie
