#FROM  openjdk:19-oraclelinux8
#RUN microdnf install git 

FROM  openjdk:16-jdk-buster
RUN useradd -ms /bin/bash vscode

RUN cd /tmp \
    && wget -q https://services.gradle.org/distributions/gradle-7.4.2-bin.zip \
    && unzip gradle-7.4.2-bin.zip -d /opt 

# Set Gradle in the environment variables
ENV GRADLE_HOME /opt/gradle-7.4.2
ENV PATH $PATH:/opt/gradle-7.4.2/bin

USER vscode
WORKDIR /home/vscode
