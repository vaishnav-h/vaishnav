# vaishnav
Scripts/Playbooks

Author: Vaishnav Harikumar
Version: 19062020

This playbook willl install ElasticSearch using RPM package from Elasticsearch repo. 
Elasticsearch depends on OpenJDK, so a conditional check for Java is also performed. 
If the command `java -version` is not found, the playbook will proceed to install java. 

Upon successfull installation, the results shows elasticsearch tagline collected from command: `curl http://localhost:9200`

Example: 

ok: [123.253.8.140] => {
    "elasticstatus.json.tagline": "You Know, for Search"
