# FROM docker.io/jenkins/jenkins:lts@sha256:01c0b0cf789fa24253090fccea264df223b5e09b14a0ea59f0847c70bdc0

# USER root
# RUN apt-get update && apt-get install -y make && apt-get install -y g++ --fix-missing
# # drop back to the regular jenkins user - good practice
# USER jenkins
FROM docker.io/jenkins/jenkins:lts


USER root

# Update package lists and install required packages
RUN apt-get update \
    && apt-get install -y make g++

# Switch back to the regular jenkins user
USER jenkins
