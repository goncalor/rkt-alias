rkt-alias
=========

rkt-alias provides you with aliases for some common [rkt][rkt-github] tasks.

[rkt-github]: https://github.com/rkt/rkt


Aliases
-------

All aliases start with `rkt-`. The rest of the alias describes more or less what the command does.

**`rkt-rm`** Removes all exited containers.

**`rkt-rmi`** Removes all images in the local store, except `stage1` images.

<!--
**`docker-stop-all`** Stops all running containers, giving them time to stop.

**`docker-force-rm-all`** Stops and them removes all containers.

**`docker-volume-rm-all`** Removes all volumes not in use.

**`docker-shark`** Stops and removes all containers and *removes all volumes*. (Be careful!)
-->

Installation
------------

Installing is as simple as downloading a file to your computer and making sure it is sourced when you log in.

### Download

Create a new directory and move into it

    mkdir -p ~/.config/rkt-alias
    cd ~/.config/rkt-alias

Download `rkt.alias` with `wget` or `curl`

    wget https://raw.githubusercontent.com/goncalor/rkt-alias/master/rkt.alias
    # or
    curl https://raw.githubusercontent.com/goncalor/rkt-alias/master/rkt.alias > rkt.alias

Go back to your original directory

    cd -

### Source

Add the following command to your `.bashrc`, `.zshrc`, or other script that suits your case

    source ~/.config/rkt-alias/rkt.alias

That will make the new aliases available the next time you open a terminal. If you want to make them available right now just run that same command on your current shell.
