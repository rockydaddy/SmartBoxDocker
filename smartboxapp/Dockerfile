# Wähle Basis Image
FROM node:latest
# Erstelle app Pfad im Container
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
#Tools und Updates
RUN ["apt-get", "update"]
#RUN ["apt-get", "install", "-y", "vim"]
RUN ["apt-get", "install", "-y", "git-core"]
# Hole Node App aus meinem Git Repo
RUN git clone https://github.com/rockydaddy/SmartBoxApp.git
# Wechsle Pfad
WORKDIR /usr/src/app/SmartBoxApp
# Installiere Node App
RUN ["npm", "install"] 
EXPOSE 80
#CMD [ "npm", "start" , "&&"]