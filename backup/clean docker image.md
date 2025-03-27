```bash
vim /etc/cron.daily/docker-prune
```
```bash
#!/bin/bash
docker image prune -a -f --filter "until=1h" && docker system prune -f
```
```bash
chmod +x /etc/cron.daily/docker-prune
```