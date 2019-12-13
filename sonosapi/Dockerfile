# Wähle Basis Image
FROM node:latest
# Erstelle app Pfad im Container
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
#Tools und Updates
RUN ["apt-get", "update"]
#RUN ["apt-get", "install", "-y", "vim"]
RUN ["apt-get", "install", "-y", "git-core"]
# Hole Node App aus Git Repo
RUN git clone https://github.com/jishi/node-sonos-http-api.git
# Wechsle Pfad
WORKDIR /usr/src/app/node-sonos-http-api
# Installiere Node App
RUN ["npm", "install", "--production"] 
EXPOSE 5005
#CMD [ "npm", "start" , "&&"]