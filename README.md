# Nextstrain Instance: the surveillance on Delta variant in Texas

Use Git to download a copy of the `ncov` repository containing the workflow.

```shell
git clone https://github.com/nextstrain/ncov.git
```

Change directory to the `ncov` directory:

```shell
cd ncov
```

Download this repository into a new subdirectory of `ncov` called `surveillanceInTexas`:

```shell
git clone https://github.com/leke-lyu/surveillanceInTexas.git
```

Replace the `lat_longs.tsv`:

```shell
rm defaults/lat_longs.tsv
cp surveillanceInTexas/lat_longs.tsv defaults/
```

From within the `ncov` directory, run the workflow using a configuration file provided in the tutorial directory:

```shell
nextstrain build . --configfile surveillanceInTexas/builds.yaml 
```
