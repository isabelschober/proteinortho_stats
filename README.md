# proteinortho_stats

This script counts Core- and Pan-genomes and strain-specific genes calculated with Proteinortho ([Lechner et al. 2011](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-12-124))

Proteinortho must have been run using the "-singles" option!

```bash
proteinortho_stats.py <my_project.proteinortho> 
```

```bash
usage: proteinortho_stats.py [-h] -p PROTEINORTHO
                             [-m {basic,input,unique,all}]

optional arguments:
  -h, --help            show this help message and exit
  -p PROTEINORTHO, --proteinortho PROTEINORTHO
                        <my_project.proteinortho> Proteinortho output
                        calculated with -singles option
  -m {basic,input,unique,all}, --mode {basic,input,unique,all}
                        What information should the script return? basic:
                        Number of input sequences, sequence type, pan- and
                        core-genome counts. input: Number of input sequences
                        per strain. unique: Number of unique sequences per
                        strain. all: all of the above. Default: basic           
```

# proteinortho_numeric

This script transforms Proteinortho ([Lechner et al. 2011](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-12-124)) output into a numeric or a binary matrix

Proteinortho must have been run using the "-singles" option!

```bash
proteinortho_numeric.py <my_project.proteinortho> 
```
```bash
usage: proteinortho_numeric.py [-h] -p PROTEINORTHO [-m {numeric,binary}]

optional arguments:
  -h, --help            show this help message and exit
  -p PROTEINORTHO, --proteinortho PROTEINORTHO
                        <my_project.proteinortho> Proteinortho output
                        calculated with -singles option
  -m {numeric,binary}, --mode {numeric,binary}
                        numeric mode gives the number of paralogs present in a
                        genome, binary mode gives out only 1 (gene family
                        present)/ 0 (gene family not present)

```

# proteinortho_curves

This script creates accumulation curves for pan- and core-genomes calculated with Proteinortho  ([Lechner et al. 2011](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-12-124))

-> [proteinortho_curves](https://github.com/isabelschober/proteinortho_curves)

