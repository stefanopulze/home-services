# Home Services Infrastructure

## Security
```bash
sudo addgroup home
# Adding group 'home' (GID 1001) ...

sudo adduser --no-create-home -gid 1001 --disabled-login mosquitto
# Adding new user `mosquitto' (1001) with group `home' ...
```

### MQTT - Mosquitto 
At first run the broker allow anonymous users.
To generate the user and password use the command 
`docker-compose exec mosquitto mosquitto_passwd -c /etc/mosquitto/passwd <user_name>`

