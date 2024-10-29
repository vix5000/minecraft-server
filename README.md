Using the configuration of project https://github.com/itzg/docker-minecraft-server

Notes: 
- Currently, server.properties file is not being used.


Requirements:
- Java JDK 21
- At least 10G of memory


Startup:
To start the server run the command `docker compose up -d` inside the directory including the docker-compose.yml file. If you want to make chandes in modpack version, edit variable CF_PAGE_URL inside the docker compose file to point to another version file.


Useful information:
- ./data includes all the information of the server


Tests:
- Kill container and see what was saved. -> Results seen: If the last player disconnects before the container is killed, the session is saved, but if the last player is online the session is not saved???
- Disconnect physical server and see what is saved (simulate power failure)
- Use whitelist -> Results seen: Whitelist is not working


Warning:
This configuration works only for curseforge modpacks.
