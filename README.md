# Author
> :wave:              Colton Smith <br>
> :computer:          Data Science Engineer <br>
> :mortar_board:      Carnegie Mellon MISM <br>
> :incoming_envelope: colton.smith.ai@gmail.com <br>
> :octocat:           https://github.com/colton-smith-ai <br>
> :date:              January 2022 <br>

# password-generator
Simple password generator, written entirely in Go, to create secure passwords.

Creates secure passwords with:
- 20 characters total :100:
- 3 symbol [!@#$<>,...] :interrobang:
- 3 number [0-9] :1234:
- 3 alphabet capital [A-Z] :arrow_up:
- 10 alphabet lowercase [a-z] :arrow_down:
- 1 random character [symbol, number, capital, or lowercase] :wink:

# Docker :whale:
Demonstrates a multistage docker image. Containers expected to be run via command line interface (cli).
Containers simply run a binary executable. Executable generates a new secure password, then displays
password on cli. Container immediately die upon displaying password. Recommended to run containers
with `--rm` option. 

- ## Recommended Docker Commands

    - ### Build Docker Image
        ` $ docker build -t password-generator https://github.com/colton-smith-ai/password-generator.git#main`

    - ### Run Image Containers
        `$ docker run --rm password-generator`

- ## Standard Docker Commands

    - ### Build Docker Image
        ` $ docker build -t image-name .`

    - ### Run Image Containers
        `$ docker run --name container-name --rm image-name`