# Docker Note in Raspberry 

### Index
1. [Install Docker in Raspberry](#install)
2. [Add `pi` account into `docker` group](#Add)
3. [Network Setting](#Network)

---

<a name="install"/>

#### 1. Install Docker in Raspberry(With Internet)

```
export VERSION=19.03.12 && curl -sSL get.docker.com | sh  
```

* You can specified docker version by setting `VERSION=XX.XX.XX`

* If you want remove docker from your raspberry, follow below command

```
sudo apt remove docker-ce
```

---

<a name="run"/>

#### 2. Add `pi` account into `docker` group

```
sudo usermod -aG docker pi
```

* pi is raspberry os default account

---

<a name="Network"/>

#### 3. Network Setting

* revise file `/etc/dhcpcd.conf`




