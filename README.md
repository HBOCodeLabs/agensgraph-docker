## AgensGraph Docker    

# Tag Info   
* **v1.3.0**, **latest** : AgensGraph v1.3.0 / debian

# Usage (docker)    
* Image download       
$ docker pull bitnine/agensgraph:v1.3.0       

* Create Volume
$ docker volume create --name myvolume

* Container starting           
    - agens 
      (Temporary mode)
      $ docker run -it bitnine/agensgraph:v1.3.0 agens
      (Save mode) 
      $ docker run -i -t -v myvolume:/home/agens/AgensGraph/data bitnine/agensgraph:v1.3.0 agens
    - bash 
      $ docker run -it bitnine/agensgraph:v1.3.0 /bin/bash

# Usage (AgensGraph)     
The image already has a graph("agens_graph"), and you can see the list of graphs created with the `\dG` command.
* list graph
agens=# \dG
* set graph
agens=#  set graph_path=[graph_name];
* show graph
agens=#  show graph_path;

# Reference
* AgensGraph Quick Guide : https://bitnine.net/documentations/quick-guide-1-3.html
* Dockfile : https://github.com/bitnine-oss/agensgraph-docker/tree/v1.3.0
# agensgraph-docker

