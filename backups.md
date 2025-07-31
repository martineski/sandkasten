# Let's Talk Backups

Here come some general notes on backups. Nobody likes to talk about them. And you can leave them off until it's too late. I'm definitely not perfect, but here go some notes about them (mostly for me to remember).

## Photos to USB

To copy my photos directory to the backup USB drive, use `rsync` like so:

```
rsync -av --ignore-existing --log-file=./my_log.txt --progress /some/source/dir/ /some/dest/dir
```

* `-a`: archive mode
* `-v`, `--progress`: add verbosity, maybe not needed
* `--ignore-existing`: skip updating files that exist on receiver
