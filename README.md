<h1 align="center">Udp2raw</h1>

<p align="center">A tunnel which turns UDP traffic into encrypted FakeTCP/UDP/ICMP traffic by using raw socket, helps you bypass UDP fireWalls(or unstable UDP environment).</p>

<p align="center">
    <a href="https://ghcr.io/akafeng/udp2raw">Container Registry</a> ·
    <a href="https://github.com/wangyu-/udp2raw-tunnel">Project Source</a>
</p>

<p align="center">
    <img src="https://img.shields.io/github/workflow/status/akafeng/docker-udp2raw/Docker%20Build" />
    <img src="https://img.shields.io/github/last-commit/akafeng/docker-udp2raw" />
    <img src="https://img.shields.io/github/v/release/akafeng/docker-udp2raw" />
    <img src="https://img.shields.io/github/release-date/akafeng/docker-udp2raw" />
</p>

---

### Pull The Image

```bash
$ docker pull ghcr.io/akafeng/udp2raw
```

### Start Container

```bash
$ docker run -d \
  --network=host \
  --restart=always \
  --name=udp2raw \
  ghcr.io/akafeng/udp2raw \
  -s \
  -l 0.0.0.0:4096 \
  -r 127.0.0.1:7777
```
