# Docker Container for Logitech Media Server (LMS)

This is a Docker image for running the Logitech Media Server package
(aka SqueezeboxServer). Currently running version v7.9.1.

Run Directly:

    docker run -d \
               -p 9000:9000 \
               -p 3483:3483 \
               -p 3483:3483/udp \
               -v <local-state-dir>:/srv/squeezebox \
               -v <audio-dir>:/srv/music \
               nephelo/docker-image-logitech-media-server
