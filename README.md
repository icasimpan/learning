# Get, build and start
```
~$ git clone --branch rust_docker git@github.com:icasimpan/learning.git rust_docker
~$ cd rust_docker
~$ cp .env-sample .env
~$ docker-compose build
~$ docker-compose up -d
```

# Shell-in
```
~$ docker-compose exec rust /bin/bash
```

# Hello Rust!
```
~$ rustc -V
rustc 1.62.1 (e092d0b6b 2022-07-16)
```

# Rust Learning Resources
* https://doc.rust-lang.org/rust-by-example/
* https://learning-rust.github.io/

# Optional
You can use docktie if you aren't too familiar with docker in the meantime - https://github.com/docktie/docktie
