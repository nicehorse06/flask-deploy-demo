[flask + gunicore + nginx deploy demo](https://www.cnblogs.com/ray-liang/p/4837850.html)

## 步驟
* uwsgi
* nginx
* supervisor
* GCP
* docker
* postresql

```
module = run:app
master = true
processes = 3

chdir = /home/horse/horse_code/flask-deploy-demo
socket = $(chdir)/uwsgi/myproject.sock
logto = $(chdir)/uwsgi/ishuhui.log
chmod-socket = 660
vacuum = true
```