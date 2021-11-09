FROM jenkins/jenkins:lts

ENV JENKINS_ADMIN_PASSWORD ""
ENV JENKINS_ADMIN_PASSWORD ""

ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false

COPY plugins_install.txt /usr/share/jenkins/ref/plugins_install.txt

RUN  jenkins-plugin-cli --plugin-file /usr/share/jenkins/ref/plugins_install.txt

COPY casc.yml /var/jenkins_home/casc.yml
