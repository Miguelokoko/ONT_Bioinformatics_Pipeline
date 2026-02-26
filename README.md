# ONT_Bioinformatics_Pipeline
## Purposely for Oxford Nanopore sequencing Technology Bioinformatics Pipeline for Anopheles mosquitoes 
### Basecalling using Dorado #### packages
```pip install dorado
pip install pod5
#### step1 Convert Fast5 Files to pod5 files
pod5 convert fast5 /input directory/*.fast5 --output/directory
pod5 convert from_fast5/ directory/*.fast5 --output/

#### converting multiple fast5 files to pod5 files
pod5 convert from_fast5 -r/directory -o/output/directory
#### step2 dorado basecaller
dorado basecaller hac /directory/*.pod5 >name.bam    ###single file
dorado basecaller hac/directory/data --recursive >name.bam```
#### Sequence alignment using Minimap2

