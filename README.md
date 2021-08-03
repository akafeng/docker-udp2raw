<h1 align="center">Udp2raw</h1>

<p align="center">A tunnel which turns UDP traffic into encrypted FakeTCP/UDP/ICMP traffic by using raw socket, helps you bypass UDP fireWalls(or unstable UDP environment).</p>

<p align="center">
    <a href="https://hub.docker.com/r/akafeng/udp2raw">Docker Hub</a> ·
    <a href="https://github.com/wangyu-/udp2raw-tunnel">Project Source</a>
</p>

<p align="center">
    <img src="https://img.shields.io/docker/v/akafeng/udp2raw?sort=semver" />
    <img src="https://img.shields.io/docker/pulls/akafeng/udp2raw" />
    <img src="https://img.shields.io/docker/image-size/akafeng/udp2raw??sort=semver" />
</p>

---

### Pull The Image

```bash
$ docker pull akafeng/udp2raw
```

### Start Container

```bash
$ docker run -d \
  --network host\
  --restart always \
  --name=udp2raw \
  akafeng/udp2raw \
  -s \
  -l 0.0.0.0:4096 \
  -r 127.0.0.1:7777
```
