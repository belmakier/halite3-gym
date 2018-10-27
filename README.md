# halite3-gym

Dockerized Halite3 Gym with a few helper scripts.

## Build the container

Assumes docker is installed and running.

```bash
cd gym
make
```

## Usage examples

Read [gym/Makefile](gym/Makefile) for examples.

## Helper script

The script [gym/halite-gym.sh](gym/halite-gym.sh) lets you execute arbitrary
commands in the container. 

## On persistence

Docker containers have no peristant storage. The helper scripts and examples
mount the folder `mnt` in the directory where they are run on the host to
`/halite` in the container.

The scripts that are stored in [gym/bin](gym/bin) expect that gym related
storage is in the folder `/halite` in the container.


# Licence

### Docker and scripts by Aqeel Akber
Unlicence. Do what you wish.

### Halite client tools

[gym/hlt_client/LICENCE](MIT licence here) and [https://github.com/HaliteChallenge/Halite-III/tree/master/tools/hlt_client/hlt_client](source repository here)

# Contributing

Leave an issue, make a suggestion, make a pull request.
