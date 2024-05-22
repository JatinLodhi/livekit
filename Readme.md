### Pre-requisites

To start, you'll need:
* A domain that you own
* The ability to add DNS records for subdomains for your new LiveKit server

### Ports to be open
Ensure that the following ports are open on your firewall and accessible on the instance:

* 443 (tcp)- primary HTTPS and TURN/TLS
* 80 (tcp)- TLS issuance
* 7881 (tcp)- WebRTC over TCP
* 3478/UDP - TURN/UDP
* 50000-60000/UDP - WebRTC over UDP
* And if Ingress is desired
* 1935 (tcp)- RTMP Ingress
* 7885/UDP - WebRTC for WHIP Ingress


### Folder architecture

#### Redis

```
redis/
├── docker-compose.yml
├── redis_data
├── logs
└── redis.conf

```

#### Sentinel

```
sentinel/
├── docker-compose.yml
├── sentinel
├── sentinel_data
└── conf
     └── sentinel.conf

```

#### Livekit

```
livekit/
├── docker-compose.yml
├── egress.yaml
├── ingress.yaml
└── livekit.yaml

```

#### Caddy

```
caddy/
├── docker-compose.yml
├── caddy.yaml
├── caddy_data

```
