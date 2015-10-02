#A Neo4j Plugin for [Dokku Alternative](https://github.com/dokku-alt/dokku-alt)
## Installing

To install the dokku-neo4j plugin:

    cd /var/lib/dokku-alt/plugins
    git clone <git url>
    dokku plugins-install


## Usage

As a pre-requisite, your app must already exist. Create a new Neo4j database by using `dokku neo4j:create appName`.  This will create a new neo4j instance and add a config variable **NEO4J\_REST\_URL** to your app's environment.

## Commands
    neo4j:create <app>                              Add Neo4j config to the app environment
    neo4j:destroy <app>                             Remove Neo4j config and container from the app environment
    neo4j:info <app>                                Shows status of Neo4j
    neo4j:link <app> <db-app>                       Link a Neo4j container from another app to this app.
    neo4j:unlink <app>                              Unlinks a Neo4j container from this app.
    neo4j:shell <app>                               Enter the neo4j-shell inside the neo4j container
    
    
## Known Issues

 - You can unlink all of the applications from a database and leave it hanging.
 
## Roadmap
 
 - Authentication Support
 - Optionally exposing the Neo4j Browser
 - Listing all neo4j databases and the apps they are linked too.
