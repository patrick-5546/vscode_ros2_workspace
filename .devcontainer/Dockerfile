FROM ghcr.io/patrick-5546/sailbot_ros2_workspace/dev

# # ** [Optional] Uncomment this section to install additional packages. **
# ENV DEBIAN_FRONTEND=noninteractive
# RUN apt-get update \
#   && apt-get -y install --no-install-recommends \
#   
#   # Clean up
#   && apt-get autoremove -y \
#   && apt-get clean -y \
#   && rm -rf /var/lib/apt/lists/*
# ENV DEBIAN_FRONTEND=dialog

# Set up auto-source of workspace for ros user
ARG WORKSPACE
# RUN echo "if [ -f ${WORKSPACE}/install/setup.bash ]; then source ${WORKSPACE}/install/setup.bash; fi" >> /home/ros/.bashrc

# Copy device-specific configuration files (e.g. .vimrc) in config/user/ to the home directory
COPY config/user ${HOME}
