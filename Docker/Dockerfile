FROM jenkins/jenkins:lts

ENV JENKINS_ADMIN_PASSWORD ""
ENV JENKINS_ADMIN_PASSWORD ""
ENV CASC_JENKINS_CONFIG /usr/local/jenkins-casc.yaml

ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false

COPY plugins_install.txt /usr/share/jenkins/ref/plugins_install.txt

RUN  jenkins-plugin-cli --plugin-file /usr/share/jenkins/ref/plugins_install.txt

COPY casc.yml "${CASC_JENKINS_CONFIG}"
