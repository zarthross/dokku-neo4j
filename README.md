#A Neo4j Plugin for Dokku
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
