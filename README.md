## 环境初始化脚本

#### Ansible 环境初始化
`ansible-playbook -i your_host_path java8.yml`

#### Java 环境初始化
`ansible-playbook -i your_host_path java8.yml`

#### Jenkins 环境初始化
`ansible-playbook -i your_host_path jenkins.yml`

#### Nodejs 初始化
`ansible-playbook -i your_host_path geerlingguy.nodejs.yml `

#### Nginx 初始化
`ansible-playbook -i your_host_path nginx.yml `

```
#! /bin/bash

docker run --rm -v /root/pgsql/bin:/root/pgsql/bin 
-v /etc/backup/data:/root/backups 
-v /etc/backup/config:/tmp -v /etc/backup/log:/log backup:latest backup perform --trigger postgres_backup 
-c /tmp/config.rb -l /log/
```

`chmod +x /etc/cron.daily/run_backup.sh`

