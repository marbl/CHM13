# Telomere-to-telomere consortium

## Introduction

We have sequenced the CHM13hTERT human cell line on the [Oxford Nanopore GridION](https://nanoporetech.com/products/gridion) using 1D ligation kits (450 bp/s) using R9.4 chemistry (FLO-MIN106). We have also sequenced approximately 50x coverage using <a href="https://www.10xgenomics.com">10X genomics</a> as well as <a href="https://bionanogenomics.com/technology/dls-technology/">BioNano DLS</a> and <a href="https://arimagenomics.com/kit/">Arima Genomics</a> HiC.

Human genomic DNA was extracted from the cultured cell line - "cells".  As the DNA is native, modified bases will be preserved. We followed the [ultra-long read (UL)  protocol](https://www.protocols.io/view/ultra-long-read-sequencing-protocol-for-rad004-mrxc57n).

# Data reuse and license

We encourage the reuse of this data in your own analysis and publications which is released under <a href="https://creativecommons.org/publicdomain/zero/1.0/">CC0</a>. While not required, we would be grateful if you would cite this github page if you find this dataset useful.

# Data
## Oxford Nanopore Data
We sequenced approximately 100 flowcells of UL data for a total of 155 Gbp (50x coverage, 1.6 Gbp/flowcell). The read N50 is 70 kbp and there are 99 Gbp of data in reads >50 kbp (32x). The longest mapping read is 1.04 Mbp. 

### rel2 (genomic DNA)

rel2 is the same data as rel1 but recalled with the latest generation callers (Guppy flip-flop 2.3.1). We have provided mappings both to our current draft assembly <!-- and to the <a href="http://ftp.1000genomes.ebi.ac.uk/vol1/ftp/technical/reference/GRCh38_reference_genome/GRCh38_full_analysis_set_plus_decoy_hla.fa">GRCh38 with decoys</a>--> in cram format, using <a href="https://github.com/lh3/minimap2">minimap2</a>.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2.fastq.gz">Guppy flip-flop 2.3.1)</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2_to_v0.4.cram">Guppy flip-flop mapped to asm v0.4 with minimap2</a>
<!--
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2_to_GRCh38.cram">Guppy flip-flop mapped to GRCh38 with decoys with minimap2</a>
-->
### rel1 (genomic DNA)

The full dataset as of 2019/01/09. These basecalls were generated on-instrument and use older versions of Guppy (depending on when the flowcell ran on the instrument). 

#### Downloads

   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel1/rel1.fastq.gz">Guppy on-instrument</a>

### fast5 data

The raw fast5 data, without basecalls, is available for completeness. The data is grouped into 96 sets.

<!--
#### Downloads

   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition001.tgz">Partition 001</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition002.tgz">Partition 002</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition003.tgz">Partition 003</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition004.tgz">Partition 004</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition005.tgz">Partition 005</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition006.tgz">Partition 006</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition007.tgz">Partition 007</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition008.tgz">Partition 008</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition009.tgz">Partition 009</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition010.tgz">Partition 010</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition011.tgz">Partition 011</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition012.tgz">Partition 012</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition013.tgz">Partition 013</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition014.tgz">Partition 014</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition015.tgz">Partition 015</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition016.tgz">Partition 016</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition017.tgz">Partition 017</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition018.tgz">Partition 018</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition019.tgz">Partition 019</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition020.tgz">Partition 020</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition021.tgz">Partition 021</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition022.tgz">Partition 022</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition023.tgz">Partition 023</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition024.tgz">Partition 024</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition025.tgz">Partition 025</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition026.tgz">Partition 026</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition027.tgz">Partition 027</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition028.tgz">Partition 028</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition029.tgz">Partition 029</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition030.tgz">Partition 030</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition031.tgz">Partition 031</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition032.tgz">Partition 032</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition033.tgz">Partition 033</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition034.tgz">Partition 034</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition035.tgz">Partition 035</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition036.tgz">Partition 036</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition037.tgz">Partition 037</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition038.tgz">Partition 038</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition039.tgz">Partition 039</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition040.tgz">Partition 040</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition041.tgz">Partition 041</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition042.tgz">Partition 042</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition043.tgz">Partition 043</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition044.tgz">Partition 044</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition045.tgz">Partition 045</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition046.tgz">Partition 046</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition047.tgz">Partition 047</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition048.tgz">Partition 048</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition049.tgz">Partition 049</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition050.tgz">Partition 050</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition051.tgz">Partition 051</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition052.tgz">Partition 052</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition053.tgz">Partition 053</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition054.tgz">Partition 054</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition055.tgz">Partition 055</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition056.tgz">Partition 056</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition057.tgz">Partition 057</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition058.tgz">Partition 058</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition059.tgz">Partition 059</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition060.tgz">Partition 060</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition061.tgz">Partition 061</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition062.tgz">Partition 062</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition063.tgz">Partition 063</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition064.tgz">Partition 064</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition065.tgz">Partition 065</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition066.tgz">Partition 066</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition067.tgz">Partition 067</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition068.tgz">Partition 068</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition069.tgz">Partition 069</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition070.tgz">Partition 070</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition071.tgz">Partition 071</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition072.tgz">Partition 072</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition073.tgz">Partition 073</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition074.tgz">Partition 074</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition075.tgz">Partition 075</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition076.tgz">Partition 076</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition077.tgz">Partition 077</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition078.tgz">Partition 078</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition079.tgz">Partition 079</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition080.tgz">Partition 080</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition081.tgz">Partition 081</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition082.tgz">Partition 082</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition083.tgz">Partition 083</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition084.tgz">Partition 084</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition085.tgz">Partition 085</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition086.tgz">Partition 086</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition087.tgz">Partition 087</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition088.tgz">Partition 088</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition089.tgz">Partition 089</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition090.tgz">Partition 090</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition091.tgz">Partition 091</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition092.tgz">Partition 092</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition093.tgz">Partition 093</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition094.tgz">Partition 094</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition095.tgz">Partition 095</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition096.tgz">Partition 096</a>
-->

## 10X Genomics Data
### Raw fastq files

Approximately 50x of data was generated on a NovaSeq instrument. Based on the summary output of <a href="https://support.10xgenomics.com/de-novo-assembly/software/overview/latest/welcome">Supernova</a>, there are 1.2 billion reads with 41x effective coverage. The mean molecule length is 130 kbp and an N50 of 864 reads per barcode.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_I1_001.fastq.gz">CHM13_prep5_S13_L002_I1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_R1_001.fastq.gz">CHM13_prep5_S13_L002_R1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_R2_001.fastq.gz">CHM13_prep5_S13_L002_R2_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_I1_001.fastq.gz">CHM13_prep5_S14_L002_I1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_R1_001.fastq.gz">CHM13_prep5_S14_L002_R1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_R2_001.fastq.gz">CHM13_prep5_S14_L002_R2_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_I1_001.fastq.gz">CHM13_prep5_S15_L002_I1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_R1_001.fastq.gz">CHM13_prep5_S15_L002_R1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_R2_001.fastq.gz">CHM13_prep5_S15_L002_R2_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_I1_001.fastq.gz">CHM13_prep5_S16_L002_I1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_R1_001.fastq.gz">CHM13_prep5_S16_L002_R1_001</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_R2_001.fastq.gz">CHM13_prep5_S16_L002_R2_001</a>

### Supernova assembly

Supernova v2.1.1 was used for assembly. The assembly is 2.95 Gbp in size with 16,903 scaffolds, a 38.5 Mbp scaffold NG50 and 210 kbp contig NG50.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/supernova/CHM13_pseudohap.1.fasta.gz">Pseudohap 1</a>
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/supernova/CHM13_pseudohap.2.fasta.gz">Pseudohap 2</a>

## BioNano DLS Data

Approximately 430x of data was generated using the Saphyr instrument and the DLE-1 enzyme. There are 15.2 M molecules with an N50 molecule length of 115.9 kbp and a max of 2.3 Mbp (2 M molecules > 150 kbp, N50 218 kbp). The assembly of the molecules is 2.97 Gbp in size with 255 contigs and an NG50 of 59.6 Mbp. 

#### Downloads

   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/bionano/chm13_Saphyr_DLE1.bnx.gz">BNX</a>
   - <a href="http://s3.amazonaws.com/nanopore-human-wgs/chm13/bionano/chm13_Saphyr_DLE1.cmap.gz">CMAP</a>

## HiC Data

The HiC raw data will be available soon.

## Previously generated PacBio data

The PacBio data was previously generated and is available from the <a href="https://www.ncbi.nlm.nih.gov/sra?linkname=bioproject_sra_all&from_uid=269593">SRA</a>

# Assembly

The current assembly draft (v0.4) is generated with [Canu v1.7.1](https://github.com/marbl/canu) including rel1 data up to 2018/11/15 and incorporating previously released [PacBio](https://www.pacb.com) data. Two gaps on the X plus the centromere were manually resolved. The assembly was polished with two rounds of [nanopolish](https://github.com/jts/nanopolish) and two rounds of [arrow](https://github.com/PacificBiosciences/GenomicConsensus). [BioNano](https://bionanogenomics.com) structural variants on the X were identified, locally mapping nanopore reads selected, reassembled, and used to patch the assembly. However, these patches are not yet polished or validated using BioNano. The assembly has not been curated outside of the X chromosome. The estimated base accuracy is QV36.

The assembly is 2.94 Gbp in size with 657 contigs and an NG50 of 85.8 Mbp

This should be considered a draft and likely has mis-assemblies, inaccurate consensus, and frame-shifted genes. It will be further validated, scaffolded with BioNano, and polished using the available data.

### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/assemblies/chm13.draft_v0.4.fasta.gz">Assembly draft v0.4</a>

# Notes on downloading files.

Files are generously hosted by Amazon Web Services. Although available as straight-forward HTTP links, download performance is improved by using the Amazon Web Services <a href="https://aws.amazon.com/cli/">command-line interface</a>. References should be amended to use the `s3://` addressing scheme, i.e. replace `http://s3.amazon.com/nanopore-human-wgs/` with `s3://nanopore-human-wgs` to download. For example, to download `rel3-nanopore-wgs-288418386-FAB39088` to the current working directory use the following command.

    aws s3 cp s3://nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_I1_001.fastq.gz .

Amending the `max_concurrent_requests` etc. settings as per <a href="http://docs.aws.amazon.com/cli/latest/topic/s3-config.html">this guide</a> will improve download performance further.

# Contact

Please raise issues on this Github repository concerning this dataset.

# History

    * rel1 and 2: 2nd March 2019. Initial release.
