# smokeping
Example docker-compose to deploy parent/child smokeping

This requires modifying the base image from linuxserver to build parent and child images. Note that
due to the bind mounting of the config directory, starting up the containers will place copies of
the config files from within the container there due to the s6 cont-init.d script.
