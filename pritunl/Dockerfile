FROM debian:jessie
RUN echo 'deb http://repo.mongodb.org/apt/debian wheezy/mongodb-org/3.0 main' > /etc/apt/sources.list.d/mongodb-org-3.0.list
RUN echo 'deb http://repo.pritunl.com/stable/apt jessie main' > /etc/apt/sources.list.d/pritunl.list
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv 7F0CEB10
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv CF8E292A
RUN apt-get update
RUN apt-get install -y pritunl mongodb-org
#RUN systemctl enable mongod pritunl
#RUN stemctl start mongod pritunl
