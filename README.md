# Nextstrain Instance: the genomic surveillance of Delta outbreak in Texas

Use Git to download a copy of the `ncov` repository containing the workflow.

```shell
git clone https://github.com/nextstrain/ncov.git --branch v12
```

Change directory to the `ncov` directory:

```shell
cd ncov
```

Download this repository into a new subdirectory of `ncov` called `surveillanceInTexas`:

```shell
git clone https://github.com/leke-lyu/surveillanceInTexas.git
```

Replace the `lat_longs.tsv` and the reference genome:

```shell
cp surveillanceInTexas/lat_longs.tsv defaults/
cp surveillanceInTexas/references_metadata.tsv data/
cp surveillanceInTexas/references_sequences.fasta data/
```
After load your data, run the workflow within the `ncov` directory using a configuration file provided in the tutorial directory:

```shell
nextstrain build . --configfile surveillanceInTexas/builds.yaml 
```
