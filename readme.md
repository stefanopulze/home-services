# Home Services Infrastructure

### MQTT - Mosquitto 
At first run the broker allow anonymous users.
To generate the user and password use the command 
`docker-compose exec mosquitto mosquitto_passwd -c /etc/mosquitto/passwd`

Next edit `config/mosquitto.conf` and set false to *allow_anonymous* and remove the comment #password_file
```
allow_anonymous false
password_file /etc/mosquitto/passwd
```

