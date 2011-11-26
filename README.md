# Digital Library's Buildout #

## Install instructions ##

I can only guarantee it'll work in **Debian 6 Lenny 64 bits**. If you're using another operational system, you're on your own.

Install system dependencies:

`[sudo] apt-get install build-essential python-setuptools python-dev zlib1g-dev libjpeg62-dev libfreetype6-dev liblcms1-dev libssl-dev libxslt1-dev`

Download and install Plone 4.0.7 in **standalone** mode.

`./install.sh standalone`

Put `buildout.cfg` and `develop.cfg` inside your `zinstance` folder, overwriting the original ones.

## Running the buildout ##

To run the buildout use:

`bin/buildout`

And, to run it in **developer** mode:

`bin/buildout -c develop.cfg`

### IMPORTANT! ###

In order to run the buildout in **developer** mode, you'll need a key to access our git repositories, as it'll clone
all the dependencies from NSI's server.
