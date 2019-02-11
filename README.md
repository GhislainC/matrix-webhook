# wifi-with-matrix

Bridge between https://code.ffdn.org/FFDN/wifi-with-me & a matrix room

## Configuration

Set the following environment variables:

- `MATRIX_URL`: the url of the matrix homeserver
- `MATRIX_ID`: the user id of the bot on this server
- `MATRIX_PW`: the password for this user
- `ROOM_ID`: the room on which send the notifications

## Dev

```
pip3 install --user matrix-client
./main.py
```

## Prod

With a proxyta.net:

```
docker-compose up -d
```

## Test

```
curl -d '{"name":"toto", "url":"http://radio.localhost/map/#44", "key": "secret"}' wwm.localhost
```
