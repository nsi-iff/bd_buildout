# Digital Library's Buildout #

## Install instructions ##

Install system dependencies:

`[sudo] apt-get install build-essential python-setuptools python-dev zlib1g-dev libjpeg62-dev libfreetype6-dev liblcms1-dev libssl-dev libxslt1-dev`

Download and install Plone 4.0.7 in **standalone** mode.

`./install.sh standalone`

Put `bd.cfg` and `bd_develop.cfg` inside your `zinstance` folder.

## Running the buildout ##

To run the buildout use:

`bin/buildout -c bd.cfg`

And, to run it in **developer** mode:

`bin/buildout -c bd_develop.cfg`

### IMPORTANT! ###

In order to run the buildout in **developer** mode, you'll need a key to access our git repositories, as it'll clone
all the dependencies from NSI's server.
