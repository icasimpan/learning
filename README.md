# Get, build and start
```
~$ git clone --branch pwsh_docker git@github.com:casimpania/learning.git pwsh_docker
~$ cd pwsh_docker
~$ cp .env-sample .env
~$ docker-compose build
~$ docker-compose up -d
```

# Shell-in
```
~$ docker-compose exec pwsh /bin/bash
```

# Hello Powershell!
```
bash-5.1$ pwsh
PowerShell 7.2.5
Copyright (c) Microsoft Corporation.

https://aka.ms/powershell
Type 'help' to get help.

PS /home/pwsh> pwsh --version
PowerShell 7.2.5
```

# Powershell Learning Resources
* https://docs.microsoft.com/en-us/powershell/ 
* https://github.com/PowerShell/PowerShell/tree/master/docs/learning-powershell
* https://github.com/PowerShell/PowerShell/blob/master/docs/learning-powershell/powershell-beginners-guide.md
* https://www.guru99.com/powershell-tutorial.html
* https://powershellonlinux.com/pages/Favorite%20Modules

# Optional
You can use docktie if you aren't too familiar with docker in the meantime - https://github.com/docktie/docktie
