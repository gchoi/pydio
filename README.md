# Pydio Cells Deployment with Docker Compose Configuration

This is a Docker Compose configuration file for Pydio Cells, a powerful file management and collaboration platform.

## 1. Deploy Pydio with Docker Compose

```bash
$ docker compose up -d
```

## 2. Open Dashboard

```bash
$ mise run dashboard:open-dashboard
```

## 3. Configure on the Dashboard

- Check "I agree with the terms"
- Next

![](./figures/01.png)

Get hostname:

```bash
$ mise run dashboard:get-hostname
[dashboard:get-hostname] $ hostname
Alexs-Mac-Studio.local # example hostname
```

- Database Connection: TCP
- HostName: {YOUR-HOSTNAME}
- Port: `3306`
- Database Name: `cells`
- Database User: `pydio`
- Password: `P@ssw0rd`

![](./figures/02.png)

- Application Title: {YOUR-APPLICATION-TITLE}
- Default Language: `English`
- Admin password: {YOUR-ADMIN-PASSWORD}
- Confirm password: {YOUR-ADMIN-PASSWORD}

![](./figures/03.png)

Install Now

![](./figures/04.png)

Installation start

![](./figures/05.png)

Login

![](./figures/06.png)

Enjoy sharing files and collaborating with others!

![](./figures/07.png)
