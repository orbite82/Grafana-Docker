## Grafana Navita:
## Work In Progess -->

* __Facilidade de subir dashboard de todo parque__
---

---
* __Configuração inicial__ 

1. __Documentção oficial__

 * Site e Documentação
  - [Link](https://grafana.com/docs/grafana/latest/installation/docker/) 

  * Docker-Compose up

  ```
   docker-compose -f docker-compose.yml up -d
  
  ```

  * Docker-Compose init all stop e restart Ec2

  ```
    root@ip-172-30-1-0:~# docker ps
    CONTAINER ID   IMAGE             COMMAND                  CREATED       STATUS       PORTS                                                  NAMES
    da706c84ec3a   portainer/agent   "./agent"                2 hours ago   Up 2 hours   0.0.0.0:9001->9001/tcp, :::9001->9001/tcp              portainer_agent
    96fa7ef203d6   grafana/grafana   "/run.sh"                2 days ago    Up 2 days    0.0.0.0:3000->3000/tcp, :::3000->3000/tcp              grafana
    a314c140ddca   mysql:5.7 

    root@ip-172-30-1-0:~# docker update --restart=always 96fa7ef203d6

  ```