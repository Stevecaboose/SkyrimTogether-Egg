FROM tiltedphoques/st-reborn-server:latest AS base

FROM alpine:latest AS final

# Note: The install script run on the container will copy the files out of this image and onto the persistent mounted storage on the Pterodactyl server.

# Copy server binaries to final image
COPY --from=base /st-server/ /home/server
