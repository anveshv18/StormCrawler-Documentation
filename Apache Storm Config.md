## Apache Storm Config

Prequesites:
- Java
- Zookeeper

**zoo.cfg**
```
tickTime=2000
initLimit=10
syncLimit=5
dataDir=/mnt/c/Users/admin/Documents/zookeeper-3.4.13
clientPort=2181
```

**storm.yaml**

```
storm.local.dir: "/mnt/c/Users/admin/Documents/apache-storm-1.2.2"
storm.zookeeper.servers: 
  - localhost
nimbus.seeds: ["localhost"]
supervisor.slots.ports: 
  - 6700
  - 6701
  - 6702
  - 6703
  ```
