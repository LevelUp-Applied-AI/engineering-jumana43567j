docker info
Client:
 Version:           29.2.1
 API version:       1.53
 Go version:        go1.25.6
 Git commit:        a5c7197
 Built:             Mon Feb  2 17:20:16 2026
 OS/Arch:           windows/amd64
 Context:           desktop-linux

Server: Docker Desktop 4.63.0 (220185)
 Engine:
  Version:          29.2.1
  API version:      1.53 (minimum version 1.44)
  Go version:       go1.25.6
  Git commit:       6bc6209
  Built:            Mon Feb  2 17:17:24 2026
  OS/Arch:          linux/amd64
  Experimental:     false
 containerd:
  Version:          v2.2.1
  GitCommit:        dea7da592f5d1d2b7755e3a161be07f43fad8f75
 runc:
  Version:          1.3.4
  GitCommit:        v1.3.4-0-gd6d73eb8
 docker-init:
  Version:          0.19.0
  GitCommit:        de40ad0
Client:
 Version:    29.2.1
 Context:    desktop-linux
 Debug Mode: false
 Plugins:
  agent: create or run AI agents (Docker Inc.)
    Version:  v1.27.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-agent.exe
  ai: Docker AI Agent - Ask Gordon (Docker Inc.)
    Version:  v1.18.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-ai.exe
  buildx: Docker Buildx (Docker Inc.)
    Version:  v0.31.1-desktop.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-buildx.exe
  compose: Docker Compose (Docker Inc.)
    Version:  v5.0.2
    Path:     C:\Program Files\Docker\cli-plugins\docker-compose.exe
  debug: Get a shell into any image or container (Docker Inc.)
    Version:  0.0.47
    Path:     C:\Program Files\Docker\cli-plugins\docker-debug.exe
  desktop: Docker Desktop commands (Docker Inc.)
    Version:  v0.3.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-desktop.exe
  extension: Manages Docker extensions (Docker Inc.)
    Version:  v0.2.31
    Path:     C:\Program Files\Docker\cli-plugins\docker-extension.exe
  init: Creates Docker-related starter files for your project (Docker Inc.)
    Version:  v1.4.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-init.exe
  mcp: Docker MCP Plugin (Docker Inc.)
    Version:  v0.40.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-mcp.exe
  model: Docker Model Runner (Docker Inc.)
    Version:  v1.1.1
    Path:     C:\Program Files\Docker\cli-plugins\docker-model.exe
  offload: Docker Offload (Docker Inc.)
    Version:  v0.5.56
    Path:     C:\Program Files\Docker\cli-plugins\docker-offload.exe
  pass: Docker Pass Secrets Manager Plugin (beta) (Docker Inc.)
    Version:  v0.0.24
    Path:     C:\Program Files\Docker\cli-plugins\docker-pass.exe
  sandbox: Docker Sandbox (Docker Inc.)
    Version:  v0.12.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-sandbox.exe
  sbom: View the packaged-based Software Bill Of Materials (SBOM) for an image Anchore Inc.)
    Version:  0.6.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-sbom.exe
  scout: Docker Scout (Docker Inc.)
    Version:  v1.20.0
    Path:     C:\Program Files\Docker\cli-plugins\docker-scout.exe

Server:
 Containers: 3
  Running: 1
  Paused: 0
  Stopped: 2
 Images: 2
 Server Version: 29.2.1
 Storage Driver: overlayfs
  driver-type: io.containerd.snapshotter.v1
 Logging Driver: json-file
 Cgroup Driver: cgroupfs
 Cgroup Version: 2
 Plugins:
  Volume: local
  Network: bridge host ipvlan macvlan null overlay
  Log: awslogs fluentd gcplogs gelf journald json-file local splunk syslog
 CDI spec directories:
  /etc/cdi
  /var/run/cdi
 Discovered Devices:
  cdi: docker.com/gpu=webgpu
 Swarm: inactive
 Runtimes: runc io.containerd.runc.v2 nvidia
 Default Runtime: runc
 Init Binary: docker-init
 containerd version: dea7da592f5d1d2b7755e3a161be07f43fad8f75
 runc version: v1.3.4-0-gd6d73eb8
 init version: de40ad0
 Security Options:
  seccomp
   Profile: builtin
  cgroupns
 Kernel Version: 6.6.87.2-microsoft-standard-WSL2
 Operating System: Docker Desktop
 OSType: linux
 Architecture: x86_64
 CPUs: 8
 Total Memory: 3.699GiB
 Name: docker-desktop
 ID: 1d975e83-7f82-4326-b64a-94c5ab200b83
 Docker Root Dir: /var/lib/docker
 Debug Mode: false
 HTTP Proxy: http.docker.internal:3128
 HTTPS Proxy: http.docker.internal:3128
 No Proxy: hubproxy.docker.internal
 Labels:
  com.docker.desktop.address=npipe://\\.\pipe\docker_cli
 Experimental: false
 Insecure Registries:
  hubproxy.docker.internal:5555
  ::1/128
  127.0.0.0/8
 Live Restore Enabled: false
 Firewall Backend: iptables


## Hello World Test
Hello from Docker!
This message shows that your installation appears to be working correctly.

To generate this message, Docker took the following steps:
 1. The Docker client contacted the Docker daemon.
 2. The Docker daemon pulled the "hello-world" image from the Docker Hub.
    (amd64)
 3. The Docker daemon created a new container from that image which runs the
    executable that produces the output you are currently reading.
 4. The Docker daemon streamed that output to the Docker client, which sent it
    to your terminal.

To try something more ambitious, you can run an Ubuntu container with:
 $ docker run -it ubuntu bash

Share images, automate workflows, and more with a free Docker ID:
 https://hub.docker.com/

For more examples and ideas, visit:
 https://docs.docker.com/get-started/

## Postgres Container
$ docker run -d \
  --name pg-prework \
  -e POSTGRES_PASSWORD=prework \
  -p 5432:5432 \
  postgres:15-alpine
6e1388fe69b0b3e23316fd338df83784962d83c531bd2444a9466f50cbd0ab49

##[paste output of: docker logs pg-prework]

The files belonging to this database system will be owned by user "postgres".
This user must also own the server process.

The database cluster will be initialized with locale "en_US.utf8".
The default database encoding has accordingly been set to "UTF8".
The default text search configuration will be set to "english".

Data page checksums are disabled.

fixing permissions on existing directory /var/lib/postgresql/data ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... posix
selecting default max_connections ... 100
selecting default shared_buffers ... 128MB
selecting default time zone ... UTC
creating configuration files ... ok
running bootstrap script ... ok
sh: locale: not found
2026-03-04 10:22:53.884 UTC [35] WARNING:  no usable system locales were found
performing post-bootstrap initialization ... ok
initdb: warning: enabling "trust" authentication for local connections
syncing data to disk ... ok
initdb: hint: You can change this by editing pg_hba.conf or using the option -A, or --auth-local and --auth-host, the next time you run initdb.


Success. You can now start the database server using:

    pg_ctl -D /var/lib/postgresql/data -l logfile start

waiting for server to start....2026-03-04 10:22:55.169 UTC [41] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 10:22:55.175 UTC [41] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 10:22:55.190 UTC [44] LOG:  database system was shut down at 2026-03-04 10:22:54 UTC
2026-03-04 10:22:55.197 UTC [41] LOG:  database system is ready to accept connections
 done
server started

/usr/local/bin/docker-entrypoint.sh: ignoring /docker-entrypoint-initdb.d/*

waiting for server to shut down...2026-03-04 10:22:55.268 UTC [41] LOG:  received fast shutdown request
.2026-03-04 10:22:55.272 UTC [41] LOG:  aborting any active transactions
2026-03-04 10:22:55.274 UTC [41] LOG:  background worker "logical replication launcher" (PID 47) exited with exit code 1
2026-03-04 10:22:55.274 UTC [42] LOG:  shutting down
2026-03-04 10:22:55.279 UTC [42] LOG:  checkpoint starting: shutdown immediate
2026-03-04 10:22:55.302 UTC [42] LOG:  checkpoint complete: wrote 3 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.007 s, sync=0.004 s, total=0.028 s; sync files=2, longest=0.002 s, average=0.002 s; distance=0 kB, estimate=0 kB
2026-03-04 10:22:55.306 UTC [41] LOG:  database system is shut down
 done
server stopped

PostgreSQL init process complete; ready for start up.

2026-03-04 10:22:55.397 UTC [1] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 10:22:55.398 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2026-03-04 10:22:55.398 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2026-03-04 10:22:55.409 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 10:22:55.418 UTC [55] LOG:  database system was shut down at 2026-03-04 10:22:55 UTC
2026-03-04 10:22:55.426 UTC [1] LOG:  database system is ready to accept connections
2026-03-04 10:27:55.283 UTC [53] LOG:  checkpoint starting: time
2026-03-04 10:27:59.417 UTC [53] LOG:  checkpoint complete: wrote 43 buffers (0.3%); 0 WAL file(s) added, 0 removed, 0 recycled; write=4.029 s, sync=0.063 s, total=4.136 s; sync files=11, longest=0.023 s, average=0.006 s; distance=252 kB, estimate=252 kB
2026-03-04 11:03:01.909 UTC [1] LOG:  received fast shutdown request
2026-03-04 11:03:01.916 UTC [1] LOG:  aborting any active transactions
2026-03-04 11:03:01.929 UTC [1] LOG:  background worker "logical replication launcher" (PID 58) exited with exit code 1
2026-03-04 11:03:01.931 UTC [53] LOG:  shutting down
2026-03-04 11:03:01.935 UTC [53] LOG:  checkpoint starting: shutdown immediate
2026-03-04 11:03:01.975 UTC [53] LOG:  checkpoint complete: wrote 0 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.019 s, sync=0.001 s, total=0.044 s; sync files=0, longest=0.000 s, average=0.000 s; distance=0 kB, estimate=227 kB
2026-03-04 11:03:01.990 UTC [1] LOG:  database system is shut down

PostgreSQL Database directory appears to contain a database; Skipping initialization

2026-03-04 11:05:03.229 UTC [1] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 11:05:03.231 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2026-03-04 11:05:03.231 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2026-03-04 11:05:03.240 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 11:05:03.258 UTC [29] LOG:  database system was shut down at 2026-03-04 11:03:01 UTC
2026-03-04 11:05:03.280 UTC [1] LOG:  database system is ready to accept connections

##[paste output of: docker stop pg-prework]
pg-prework

##[paste output of: docker restart pg-prework]
pg-prework

##[paste output of: docker logs pg-prework (after restart)]
The files belonging to this database system will be owned by user "postgres".
This user must also own the server process.

The database cluster will be initialized with locale "en_US.utf8".
The default database encoding has accordingly been set to "UTF8".
The default text search configuration will be set to "english".

Data page checksums are disabled.

fixing permissions on existing directory /var/lib/postgresql/data ... ok
creating subdirectories ... ok
selecting dynamic shared memory implementation ... posix
selecting default max_connections ... 100
selecting default shared_buffers ... 128MB
selecting default time zone ... UTC
creating configuration files ... ok
running bootstrap script ... ok
sh: locale: not found
2026-03-04 10:22:53.884 UTC [35] WARNING:  no usable system locales were found
performing post-bootstrap initialization ... ok
initdb: warning: enabling "trust" authentication for local connections
syncing data to disk ... ok
initdb: hint: You can change this by editing pg_hba.conf or using the option -A, or --auth-local and --auth-host, the next time you run initdb.


Success. You can now start the database server using:

    pg_ctl -D /var/lib/postgresql/data -l logfile start

waiting for server to start....2026-03-04 10:22:55.169 UTC [41] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 10:22:55.175 UTC [41] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 10:22:55.190 UTC [44] LOG:  database system was shut down at 2026-03-04 10:22:54 UTC
2026-03-04 10:22:55.197 UTC [41] LOG:  database system is ready to accept connections
 done
server started

/usr/local/bin/docker-entrypoint.sh: ignoring /docker-entrypoint-initdb.d/*

waiting for server to shut down...2026-03-04 10:22:55.268 UTC [41] LOG:  received fast shutdown request
.2026-03-04 10:22:55.272 UTC [41] LOG:  aborting any active transactions
2026-03-04 10:22:55.274 UTC [41] LOG:  background worker "logical replication launcher" (PID 47) exited with exit code 1
2026-03-04 10:22:55.274 UTC [42] LOG:  shutting down
2026-03-04 10:22:55.279 UTC [42] LOG:  checkpoint starting: shutdown immediate
2026-03-04 10:22:55.302 UTC [42] LOG:  checkpoint complete: wrote 3 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.007 s, sync=0.004 s, total=0.028 s; sync files=2, longest=0.002 s, average=0.002 s; distance=0 kB, estimate=0 kB
2026-03-04 10:22:55.306 UTC [41] LOG:  database system is shut down
 done
server stopped

PostgreSQL init process complete; ready for start up.

2026-03-04 10:22:55.397 UTC [1] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 10:22:55.398 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2026-03-04 10:22:55.398 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2026-03-04 10:22:55.409 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 10:22:55.418 UTC [55] LOG:  database system was shut down at 2026-03-04 10:22:55 UTC
2026-03-04 10:22:55.426 UTC [1] LOG:  database system is ready to accept connections
2026-03-04 10:27:55.283 UTC [53] LOG:  checkpoint starting: time
2026-03-04 10:27:59.417 UTC [53] LOG:  checkpoint complete: wrote 43 buffers (0.3%); 0 WAL file(s) added, 0 removed, 0 recycled; write=4.029 s, sync=0.063 s, total=4.136 s; sync files=11, longest=0.023 s, average=0.006 s; distance=252 kB, estimate=252 kB
2026-03-04 11:03:01.909 UTC [1] LOG:  received fast shutdown request
2026-03-04 11:03:01.916 UTC [1] LOG:  aborting any active transactions
2026-03-04 11:03:01.929 UTC [1] LOG:  background worker "logical replication launcher" (PID 58) exited with exit code 1
2026-03-04 11:03:01.931 UTC [53] LOG:  shutting down
2026-03-04 11:03:01.935 UTC [53] LOG:  checkpoint starting: shutdown immediate
2026-03-04 11:03:01.975 UTC [53] LOG:  checkpoint complete: wrote 0 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.019 s, sync=0.001 s, total=0.044 s; sync files=0, longest=0.000 s, average=0.000 s; distance=0 kB, estimate=227 kB
2026-03-04 11:03:01.990 UTC [1] LOG:  database system is shut down

PostgreSQL Database directory appears to contain a database; Skipping initialization

2026-03-04 11:05:03.229 UTC [1] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 11:05:03.231 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2026-03-04 11:05:03.231 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2026-03-04 11:05:03.240 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 11:05:03.258 UTC [29] LOG:  database system was shut down at 2026-03-04 11:03:01 UTC
2026-03-04 11:05:03.280 UTC [1] LOG:  database system is ready to accept connections
2026-03-04 11:10:03.105 UTC [27] LOG:  checkpoint starting: time
2026-03-04 11:10:03.179 UTC [27] LOG:  checkpoint complete: wrote 3 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.023 s, sync=0.011 s, total=0.074 s; sync files=2, longest=0.006 s, average=0.006 s; distance=0 kB, estimate=0 kB
2026-03-04 11:18:27.267 UTC [1] LOG:  received fast shutdown request
2026-03-04 11:18:27.270 UTC [1] LOG:  aborting any active transactions
2026-03-04 11:18:27.278 UTC [1] LOG:  background worker "logical replication launcher" (PID 32) exited with exit code 1
2026-03-04 11:18:27.278 UTC [27] LOG:  shutting down
2026-03-04 11:18:27.282 UTC [27] LOG:  checkpoint starting: shutdown immediate
2026-03-04 11:18:27.308 UTC [27] LOG:  checkpoint complete: wrote 0 buffers (0.0%); 0 WAL file(s) added, 0 removed, 0 recycled; write=0.009 s, sync=0.001 s, total=0.029 s; sync files=0, longest=0.000 s, average=0.000 s; distance=0 kB, estimate=0 kB
2026-03-04 11:18:27.319 UTC [1] LOG:  database system is shut down

PostgreSQL Database directory appears to contain a database; Skipping initialization

2026-03-04 11:19:26.888 UTC [1] LOG:  starting PostgreSQL 15.17 on x86_64-pc-linux-musl, compiled by gcc (Alpine 15.2.0) 15.2.0, 64-bit
2026-03-04 11:19:26.891 UTC [1] LOG:  listening on IPv4 address "0.0.0.0", port 5432
2026-03-04 11:19:26.891 UTC [1] LOG:  listening on IPv6 address "::", port 5432
2026-03-04 11:19:26.899 UTC [1] LOG:  listening on Unix socket "/var/run/postgresql/.s.PGSQL.5432"
2026-03-04 11:19:26.912 UTC [29] LOG:  database system was shut down at 2026-03-04 11:18:27 UTC
2026-03-04 11:19:26.927 UTC [1] LOG:  database system is ready to accept connections

