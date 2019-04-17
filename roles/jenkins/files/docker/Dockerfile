FROM jenkins/jenkins:lts

USER root
RUN  curl -fsSL get.docker.com -o get-docker.sh && \
     sh get-docker.sh && \
     usermod -aG docker jenkins

USER jenkins

# Skip initial setup
ENV JENKINS_OPTS -Djenkins.install.runSetupWizard=false

