# Python tools

Small talk about useful tools written in Python at
[VigoJUG](https://meetup.com/es-ES/VigoJUG/events/255662689/) meetup in November 8, 2018.

To reproduce it with [*asciinema*](https://asciinema.org):

```
$ asciinema play python-tools.cast
```

* pipsi https://github.com/mitsuhiko/pipsi

Installing
```
curl https://raw.githubusercontent.com/mitsuhiko/pipsi/master/get-pipsi.py | python
tree /home/alex/.local/ -L 2

```

```
/home/alex/.local
├── bin
│   ├── pipsi -> /home/alex/.local/venvs/pipsi/bin/pipsi
├── share
│   └── virtualenvs
└── venvs
    ├── pipsi
    ├── ansible
    ├── asciinema
    ├── httpie
    ├── pgcli
    ├── watchdog
    └── youtube-dl
```

* httpie https://httpie.org/

Installing
```
    pipsi install ansible
    pipsi install httpie
```

```
http http://www.local.test/secciones.php\?sec\=descargas\&ap\=contar\&tabla\=musica\&id\=7700\&link_bajar\=1 | grep "\.torrent"
http --download http://www.local.test/uploads/tmp/torrent.php\?table\=musica/\&name\=Music_Collection.torrent

http https://httpbin.org/json
http https://httpbin.org/xml
```

* youtube-dl https://youtube-dl.org/

```pipsi install youtube-dl
   youtube-dl --extract-audio --audio-format mp3 https://www.youtube.com/watch?v=FzG4uDgje3M
   ll
```


* watchdog https://pythonhosted.org/watchdog/

```
    pipsi install watchdog
    watchmedo shell-command --drop --ignore-directories --recursive --patterns="*.mp3;"  --command='cowsay -f head-in "Xa tes a tua descarga lista :-)"' .
    Ctrl+B %
    ll
    youtube-dl --extract-audio --audio-format mp3 https://www.youtube.com/watch?v=KCmw-wEizI4

```

* pgcli https://github.com/dbcli/pgcli

```
    pipsi install pgcli
    pgcli pythontools
```

* asciinema https://asciinema.org

```
    pipsi install --python python3.6 asciinema
```

