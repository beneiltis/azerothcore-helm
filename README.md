Architecture Overview:
```
                         +--------------+
                         |              |
                         |  Game Client |
                         |              |
                         +--------------+
                                 |
                +----------------+----------------------------+
                |                                             |
     +--------------------+          +------------------+     |
     |                    |          |                  |     |
     |     Auth-Server    |<-------->|  NFS-Server      |     |
     |                    |          |  (Shared Data)   |     |
     +--------------------+          +------------------+     |
                |                              |              |
                |                              |              |
                v                              v              |
     +--------------------+          +------------------+     |
     |                    |          |                  |     |
     |    MySQL-Database  |<-------->|    World-Server  |<----+
     |                    |          |                  |
     +--------------------+          +------------------+
```
