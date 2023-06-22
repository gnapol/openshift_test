FROM jenkins/jenkins:latest

USER root

# Installation de dépendances supplémentaires, le cas échéant

# Configuration des plugins Jenkins recommandés
RUN /usr/local/bin/install-plugins.sh \
    docker-plugin \
    # Ajoutez ici d'autres plugins nécessaires

# Configuration initiale de Jenkins (facultative)
COPY init.groovy /usr/share/jenkins/ref/init.groovy.d/

# Configuration supplémentaire de Jenkins (facultative)
# COPY config.xml /var/jenkins_home/config.xml

# Configuration du nombre de workers (facultatif)
# COPY jenkins.properties /usr/share/jenkins/ref/jenkins.properties

USER jenkins

