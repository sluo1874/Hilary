# Hilary

The NodeJS implementation of Sakai OAE
<br/>
## Quickstart guide

The following guide will take you through the necessary steps to set up the back-end for Sakai OAE.<br/>Start by forking and cloning the repository onto your local machine, instructions can be found [here](https://help.github.com/articles/fork-a-repo).
<br/>
### Installing node.js
Download and install the latest version of [node.js](http://nodejs.org/).<br/>
### Installing dependancies
Once you have successfully cloned the repository and installed node.js, run the following commands in order to install all required dependancies.
More information about npm can be found [here](https://npmjs.org/).<br/>
```
cd your-sakai-repo-dir
npm install -d
```
### Setting up Cassandra
Download and install the latest version of [cassandra](http://cassandra.apache.org/).
Once downloaded and extracted in a directory of your choice, run the following commands to create the necessary folders that cassandra needs to run.<br/>
```
cd your-cassandra-dir
sudo mkdir -p /var/log/cassandra
sudo chown -R `whoami` /var/log/cassandra
sudo mkdir -p /var/lib/cassandra
sudo chown -R `whoami` /var/lib/cassandra
```
### Running the server
All that remains now is booting the server.<br/>
#### Start Cassandra
```
cd your-cassandra-dir
bin/cassandra -f
```
#### Start Hilary
```
cd your-sakai-repo-dir
node app.js
```
<br/>
And that's it, the server should now be up and running!<br/>
We're looking forward to seeing your contributions to the Sakai OAE project!
