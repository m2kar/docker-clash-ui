# docker-clash-ui
clash with clash-dashboard located at `/ui`.

Run clash in docker under [the official instructions](https://github.com/Dreamacro/clash/wiki/Run-clash-in-docker).

```
docker run -itd --rm --name clash -p 7890:7890 -p 7891:7891 -p 9090:9090 -v ${PWD}/clash.yaml:/root/.config/clash/config.yaml:ro dreamacro/clash
```

but remember to add one line
```
external-ui: /ui
```
to your `config.yml`.
