# Flask Crime Map

Flask Crime Map Project taken from Flask By Example Ebook

---

1. Install Requirements
```bash
$ pip install -r requirements.txt
```

2. Install Apache2, mod_wsgi, Git and MySQL Server
```bash
$ sudo apt-get install apache2 libapache2-mod-wsgi git mysql-server
```

3. Clone this repo to `/var/www/` directory
```bash
$ git clone https://github.com/repodevs/flask-crimemap.git /var/www/flask-crimemap
```

4. Copy this `apache2/crimemap.conf` config to `site-available` apache2 directory
```bash
$ sudo cp apache2/crimemap.conf /etc/apache2/sites-available/
```

5. Enable configuration and disable default apache2 configuration
```bash
# disable default conf, or disable other conf
$ sudo a2dissite 000-default.conf
$ sudo a2ensite crimemap.conf
$ sudo service apache2 reload
```

6. Open in your browser [http://127.0.0.1](http://127.0.0.1)

