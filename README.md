# Telomere-to-telomere consortium

## Introduction

We have sequenced the CHM13hTERT human cell line on the [Oxford Nanopore GridION](https://nanoporetech.com/products/gridion) using 1D ligation kits (450 bp/s) using R9.4 chemistry (FLO-MIN106). We have also sequenced approximately 50x coverage using <a href="https://www.10xgenomics.com">:10X genomics</a> as well as <a href="https://bionanogenomics.com/technology/dls-technology/">BioNano DLS</a> and <a href="https://arimagenomics.com/kit/">Arima Genomics</a> HiC.

Human genomic DNA was extracted from the cultured cell line - "cells".  As the DNA is native, modified bases will be preserved. We followed the [ultra-long read (UL)  protocol](https://www.protocols.io/view/ultra-long-read-sequencing-protocol-for-rad004-mrxc57n).

# Data reuse and license

We encourage the reuse of this data in your own analysis and publications which is released under the Creative Commons CC-BY license. Therefore we would be grateful if you would cite the reference below if you do.

# Citation

# Data
## Oxford Nanopore Data
We sequenced approximately 100 flowcells of UL data for a total of 155 Gbp (50x coverage, 1.6 Gbp/flowcell). The read N50 is 70 kbp and there are 99 Gbp of data in reads >50 kbp (32x). The longest mapping read is 1.04 Mbp. 

### rel2 (genomic DNA)

rel2 is the same data as rel1 but recalled with the latest generation callers (Guppy flip-flop 2.3.1). We have provided mappings both to our current draft assembly and to the <a href="http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/technical/reference/GRCh38_reference_genome/GRCh38_full_analysis_set_plus_decoy_hla.fa">=GRCh38 with decoys</a> in cram format, using <a href="https://github.com/lh3/minimap2">minimap2</a>.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/rel2/flip-flop.fastq.gz">Guppy flip-flop 2.3.1)</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/rel2/flip-flop.v0.5.cram">Guppy flip-flop mapped to asm v0.5 with minimap2</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/rel2/flip-flop.v0.5.cram">Guppy flip-flop mapped to GRCh38 with decoys with minimap2</a>

### rel1 (genomic DNA)

The full dataset as of 2019/01/09. These basecalls were generated on-instrument and use an older version of Guppy. 

#### Downloads

   - <a href="http://s3.amazonaws.com/chm13/rel1/albacore.fastq.gz">Guppy on-instrument</a>

### fast5 data

The raw fast5 data, without basecalls, is available for completeness. The data is grouped into 94 read sets.

#### Downloads

   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>
   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>
   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>


## 10X Genomics Data
### Raw fastq files

Approximately 50x of data was generated on a NovaSeq instrument. Based on the summary output of <a href="https://support.10xgenomics.com/de-novo-assembly/software/overview/latest/welcome">Supernova</a>, there are 1.2 billion reads with 41x effective coverage. The mean molecule length is 130 kbp and an N50 of 864 reads per barcode.

#### Downloads

   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>

### Supernova assembly

Supernova v2.1.1 was used for assembly. The assembly is 2.95 Gbp in size with 16,903 scaffolds, a 38.5 Mbp scaffold NG50 and 210 kbp contig N50.

#### Downloads

   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>


## BioNano DLS Data

The raw moleclues (in bnx format) as well as the BioNano assembly (in cmap format) will be available soon.

#### Downloads

   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>
   - <a href="http://s3.amazonaws.com/chm13/fast5/flowcell1.tgz">Flowcell 1</a>

## HiC Data

The HiC raw data will be available soon.

# Assembly

The current assembly draft (v0.5) is generated with (Canu v1.7.1)[https://github.com/marbl/canu] including rel1 data up to 2018/11/15 and incorporating [previously released](https://www.ncbi.nlm.nih.gov/sra?linkname=bioproject_sra_all&from_uid=269593) [PacBio](https://www.pacb.com) data. Two gaps on the X plus the centromere were manually resolved. The assembly was polished with two rounds of [nanopolish](https://github.com/jts/nanopolish) and two rounds of [arrow](https://github.com/PacificBiosciences/GenomicConsensus). [BioNano](https://bionanogenomics.com) structural variants on the X were identified and patched. However, these patches are not yet polished. 

The assembly is 2.94 Gbp in size with 657 contigs and an NG50 of 85.8 Mbp

This should be considered a draft and will be further validated, scaffolded with BioNano, and further polished using the available data.

### Downloads


   - <a href="http://s3.amazonaws.com/chm13/asm/chm13_v0.5.fasta.gz>Assembly draft v0.5</a>
