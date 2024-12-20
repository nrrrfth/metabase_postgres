# Setup Postgresql
1. Perhatikan, apabila terdapat postgres dalam komputer/perangkat kamu, port 5432 sudah dipakai. Maka dari itu, ganti port selain 5432 (misal; 5433)
2. Pada `docker-compose.yml`, berikan nilai `port` seperti ini `port : "port_baru:5432`

# Setup Metabase
1. Pada `docker-compose.yml`, `host_db_port` adalah `5432`, kecuali diluar docker. Seperti DBeaver yang akan membuka database postgre yang ada di docker. DBeaver kita akan kita arahkan menggunakan port `port_baru`
1. Host database dikarenakan berada di docker lokal, maka pakai nama host `host.docker.internal`
