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

rel2 is the same data as rel1 but recalled with the latest generation callers (Guppy flip-flop 2.3.1). We have provided mappings both to our current draft assembly <!-- and to the <a href="https://ftp.1000genomes.ebi.ac.uk/vol1/ftp/technical/reference/GRCh38_reference_genome/GRCh38_full_analysis_set_plus_decoy_hla.fa">GRCh38 with decoys</a>--> in cram format, using <a href="https://github.com/lh3/minimap2">minimap2</a>.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2.fastq.gz">Guppy flip-flop 2.3.1</a> (md5: 26s7e3f4ded02d500a3db0c76c84cdc42b9)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2_to_v0.4.cram">Guppy flip-flop mapped to asm v0.4 with minimap2</a> (md5: 09d87ae044d1628056cb95690dc93378)
<!--
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel2/rel2_to_GRCh38.cram">Guppy flip-flop mapped to GRCh38 with decoys with minimap2</a>
-->
### rel1 (genomic DNA)

The full dataset as of 2019/01/09. These basecalls were generated on-instrument and use older versions of Guppy (depending on when the flowcell ran on the instrument). 

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/rel1/rel1.fastq.gz">Guppy on-instrument</a> (md5: c2cb74601eb657df21b7d25980908288)

### fast5 data

The raw fast5 data, without basecalls, is available for completeness. The data is grouped into 96 sets.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition001.tgz">Partition 001</a> (md5: c837460c50a4446fc8320c95dc88f204)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition002.tgz">Partition 002</a> (md5: 05ceccf4256d248aaec2a4c61e58c26c)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition003.tgz">Partition 003</a> (md5: 879e3a6391e5da5f943fa46b92decd47)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition004.tgz">Partition 004</a> (md5: 600bfa46c741eeff0064b1d8040b9349)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition005.tgz">Partition 005</a> (md5: 1a72beff4b2e4556c5033176ed1cd109)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition006.tgz">Partition 006</a> (md5: fcd6f8ceeac2034eddaa33cedf6d0010)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition007.tgz">Partition 007</a> (md5: 0d44cb41a4888b55bce2cba7e70107ba)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition008.tgz">Partition 008</a> (md5: 52242770505ac9aca1070e0b926c4769)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition009.tgz">Partition 009</a> (md5: 4e85e63a4ebf8efb2f97fdcee46e5737)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition010.tgz">Partition 010</a> (md5: e495530dd8a68b7bc9864ab89a4ef52f)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition011.tgz">Partition 011</a> (md5: 3b57e6256d0162d83a281e74157134e0)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition012.tgz">Partition 012</a> (md5: 735a0a03c6bec1e0ed417baa0c2d7db2)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition013.tgz">Partition 013</a> (md5: 90c51a9ab06266b2a980bcc16d3d3960)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition014.tgz">Partition 014</a> (md5: 645ea0b4edc2bfc71c708a53d5b0d92b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition015.tgz">Partition 015</a> (md5: 24f456adb4c1c6579fe34f07c82179e7)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition016.tgz">Partition 016</a> (md5: 6b72ddda5a7a1c10b50f3026914519ec)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition017.tgz">Partition 017</a> (md5: 14e7b918b28ecc784b68569454fa27d9)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition018.tgz">Partition 018</a> (md5: d5f7c9b1d88cf48298f6cbbb2a2a45a9)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition019.tgz">Partition 019</a> (md5: cefa121a627dfcf9a1dfb117065a7264)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition020.tgz">Partition 020</a> (md5: ca0729b28cd4cccc81eba670c6e86689)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition021.tgz">Partition 021</a> (md5: 51a873a2019f2b091ab035cc3f074bb8)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition022.tgz">Partition 022</a> (md5: e9235f052d651b4ba1fdaaa06ad134d0)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition023.tgz">Partition 023</a> (md5: 75ebfdb40745d667962a19a0aa838837)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition024.tgz">Partition 024</a> (md5: e1e05425f9823e50650bd2cf1efa41c6)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition025.tgz">Partition 025</a> (md5: f8efb23a5e77b12f46bce73b2ddba36a)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition026.tgz">Partition 026</a> (md5: 829f32786514b092da9e4fb8701da037)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition027.tgz">Partition 027</a> (md5: 15ebb086d975583386c1d0e49fbca932)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition028.tgz">Partition 028</a> (md5: 3dd39dee6efea9b1b50d282d1d2aae19)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition029.tgz">Partition 029</a> (md5: 3c5b3522dd741214554f84d8645cdf20)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition030.tgz">Partition 030</a> (md5: 1ef7fe24c315085d8dcfe4e6ba9b4de2)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition031.tgz">Partition 031</a> (md5: e9501d4d0fd38d64c2ad1c81f8d1a0e3)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition032.tgz">Partition 032</a> (md5: 1f3ff51da0e87c2009bef8256b930f0b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition033.tgz">Partition 033</a> (md5: 76a518084b021db82fd5dab7540e88bb)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition034.tgz">Partition 034</a> (md5: fd9f4dcfaeb89134a4f700a5346c16fa)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition035.tgz">Partition 035</a> (md5: dbdd53ba61d67a7f61405ae39d2b931b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition036.tgz">Partition 036</a> (md5: c243b8f64bde0051fe104e8baaecf09b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition037.tgz">Partition 037</a> (md5: aafa1d558881b2b4856fde3af0cbb9b2)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition038.tgz">Partition 038</a> (md5: d2e39e42eaf6a0a63d0542435590dd88)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition039.tgz">Partition 039</a> (md5: ef48d5c46f19de02fb6f6646726c95de)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition040.tgz">Partition 040</a> (md5: 17d7d34b45e14b2a79fc30e5c5084315)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition041.tgz">Partition 041</a> (md5: eb6a16d0b37d538bdbf90c3bfcc0f098)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition042.tgz">Partition 042</a> (md5: 7dbf87d75c901463b2e4e4afdc4adb52)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition043.tgz">Partition 043</a> (md5: 97c071a1d0a170e9f4809f6cdc459a6b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition044.tgz">Partition 044</a> (md5: 27dc707435a2c98fc7201ccefec68c9d)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition045.tgz">Partition 045</a> (md5: 54ce28e1e1b54ab9fd8dd072711acd30)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition046.tgz">Partition 046</a> (md5: b174c7826fc399312fad331660745e55)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition047.tgz">Partition 047</a> (md5: 2b6ce400051fce5d2de09fd8fd461fc8)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition048.tgz">Partition 048</a> (md5: 81415b29f2b6a605473af6d3529758b1)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition049.tgz">Partition 049</a> (md5: ffc9182d8a9ad9752b6571d3d2f2b69d)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition050.tgz">Partition 050</a> (md5: 790281fcf0512a798b6f0e75b14620be)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition051.tgz">Partition 051</a> (md5: 4fc5dc17819a3727e5cedaa89550ef9f)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition052.tgz">Partition 052</a> (md5: d33a70e926dee0e67cf1a75d50ee1249)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition053.tgz">Partition 053</a> (md5: 9d66e1372866dd454173f486d57ae322)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition054.tgz">Partition 054</a> (md5: 958b62e07349258d93ee3e089c6f91ff)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition055.tgz">Partition 055</a> (md5: 0e605a04d9bbeb0573aefddbfae12bd6)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition056.tgz">Partition 056</a> (md5: 29b205c649f66e3d44ea9f598b492bc2)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition057.tgz">Partition 057</a> (md5: 7336b91e333ae912b4cfc6e366570c54)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition058.tgz">Partition 058</a> (md5: 2d992482005a2523f710487f2c0a0a31)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition059.tgz">Partition 059</a> (md5: 3b45c205982796a90aa0f40955c4937b)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition060.tgz">Partition 060</a> (md5: f085ae6a4818c44d03a6f5adfc445699)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition061.tgz">Partition 061</a> (md5: 1c5a3a0ed8b53a930535b9d34e6a0667)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition062.tgz">Partition 062</a> (md5: fbfd4ffb7cf8fca4d613d0ec67d3104c)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition063.tgz">Partition 063</a> (md5: 9ddf7a9fe7e9cf8ceb02b8debed41fcc)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition064.tgz">Partition 064</a> (md5: ee3ac8080a19d4a6ab3af84074d03d7a)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition065.tgz">Partition 065</a> (md5: d94a12692d399c44612cab8b2aea8164)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition066.tgz">Partition 066</a> (md5: a9f3bfa69bbc248b33f99f42827331eb)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition067.tgz">Partition 067</a> (md5: 6c9d4b38edc6f78521f3cfdd8edc571c)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition068.tgz">Partition 068</a> (md5: 76a29683bfad7c4a0b8a0bdbbbd6fd49)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition069.tgz">Partition 069</a> (md5: f924667636c528d56e46aa92db0a182d)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition070.tgz">Partition 070</a> (md5: f813b0a4b2a4a2353c7deb539f16f286)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition071.tgz">Partition 071</a> (md5: fa56e2524ea2cc57e79f692466375b83)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition072.tgz">Partition 072</a> (md5: 23b1df220d55ab9df2735c74849a53c9)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition073.tgz">Partition 073</a> (md5: 70839cbc61d3d8af7fafcb7ba8f96461)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition074.tgz">Partition 074</a> (md5: 109b91ceda32ab0f8b9edb24cb35fb23)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition075.tgz">Partition 075</a> (md5: 53c466af09a3a119df3255189091bcda)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition076.tgz">Partition 076</a> (md5: 22ad2327db64767e34378508afe60706)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition077.tgz">Partition 077</a> (md5: 64c7c1702e3476137c54ebc0c07d970e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition078.tgz">Partition 078</a> (md5: 6e2048a8a2ceb36bb679455e0af81230)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition079.tgz">Partition 079</a> (md5: 45717c24fe844f2605be81bd8e15d856)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition080.tgz">Partition 080</a> (md5: 1ac20637828f0f3115f1c0f289e006aa)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition081.tgz">Partition 081</a> (md5: e7b5e584de5f2cbda1d53ec2f6e2668e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition082.tgz">Partition 082</a> (md5: aad214d168ad3a59488dfac71fcedc22)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition083.tgz">Partition 083</a> (md5: d557dee3b08c61d540fd6a00689341fa)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition084.tgz">Partition 084</a> (md5: cc2b4676515b988dd4f64724e49c3304)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition085.tgz">Partition 085</a> (md5: 34e6154991e5d5c641e22a529c5f06e1)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition086.tgz">Partition 086</a> (md5: 2f9ff4371f32c3a33ea081ad8825437e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition087.tgz">Partition 087</a> (md5: 945504e89ba54cdab032eac63985d216)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition088.tgz">Partition 088</a> (md5: 46a8ba05cb12b268c7f7ce04575d24da)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition089.tgz">Partition 089</a> (md5: 5fd0219c9c99aa08ce07bb35e647144c)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition090.tgz">Partition 090</a> (md5: da0e3f19f81c99a89bcff7e8f74dc6cb)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition091.tgz">Partition 091</a> (md5: c11b11f3386d47dd33acc3cba7f44fb2)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition092.tgz">Partition 092</a> (md5: 87dfa60ae9308214b43aa7075ddd9f44)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition093.tgz">Partition 093</a> (md5: 6eced035881d3e804bea7103d26c042e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition094.tgz">Partition 094</a> (md5: 59ebbc64994779244e5f7431c54b819e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition095.tgz">Partition 095</a> (md5: 4de3c1f5163357a256847c1082379df3)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/nanopore/fast5/partition096.tgz">Partition 096</a> (md5: cf16e88c803b82b052651171490d6d5a)

## 10X Genomics Data
### Raw fastq files

Approximately 50x of data was generated on a NovaSeq instrument. Based on the summary output of <a href="https://support.10xgenomics.com/de-novo-assembly/software/overview/latest/welcome">Supernova</a>, there are 1.2 billion reads with 41x effective coverage. The mean molecule length is 130 kbp and an N50 of 864 reads per barcode.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_I1_001.fastq.gz">CHM13_prep5_S13_L002_I1_001</a> (md5: 84af4586ca9f78060d5802b36cdd9e8a)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_R1_001.fastq.gz">CHM13_prep5_S13_L002_R1_001</a> (md5: 231633e0cf2fbdeba732dc7ad6233fa0)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_R2_001.fastq.gz">CHM13_prep5_S13_L002_R2_001</a> (md5: 386febfc3fc760e11e315e69310ed3d8)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_I1_001.fastq.gz">CHM13_prep5_S14_L002_I1_001</a> (md5: f0b7628e90dfaf2f702ec613c7b61ca7)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_R1_001.fastq.gz">CHM13_prep5_S14_L002_R1_001</a> (md5: 86afbc7a41ea1c81657bf1ca64d1178c)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S14_L002_R2_001.fastq.gz">CHM13_prep5_S14_L002_R2_001</a> (md5: 3dfbe58b5ae715213e20614837dcf3b7)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_I1_001.fastq.gz">CHM13_prep5_S15_L002_I1_001</a> (md5: ee34f03c765787ea069050d8eaac1de4)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_R1_001.fastq.gz">CHM13_prep5_S15_L002_R1_001</a> (md5: 73edcb56dd18d7b7b2705b4db7b4efc5) 
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S15_L002_R2_001.fastq.gz">CHM13_prep5_S15_L002_R2_001</a> (md5: a0de8e5bc127203129e4e1437b3e6aaa)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_I1_001.fastq.gz">CHM13_prep5_S16_L002_I1_001</a> (md5: 42db246f7e5725a7b6ff3f5f5aedfd6e)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_R1_001.fastq.gz">CHM13_prep5_S16_L002_R1_001</a> (md5: 3d3db7eccaf388fbcd901cbc6ad47630)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/CHM13_prep5_S16_L002_R2_001.fastq.gz">CHM13_prep5_S16_L002_R2_001</a> (md5: 9dfcc17398a7acd906212a09ab4c8903)

### Supernova assembly

Supernova v2.1.1 was used for assembly. The assembly is 2.95 Gbp in size with 16,903 scaffolds, a 38.5 Mbp scaffold NG50 and 210 kbp contig NG50.

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/supernova/CHM13_pseudohap.1.fasta.gz">Pseudohap 1</a> (md5: 6c9760ac5154072e137729b4fff18c8a)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/10x/supernova/CHM13_pseudohap.2.fasta.gz">Pseudohap 2</a> (md5: e17d89752ee458310418f207bffe4241)

## BioNano DLS Data

Approximately 430x of data was generated using the Saphyr instrument and the DLE-1 enzyme. There are 15.2 M molecules with an N50 molecule length of 115.9 kbp and a max of 2.3 Mbp (2 M molecules > 150 kbp, N50 218 kbp). The assembly of the molecules is 2.97 Gbp in size with 255 contigs and an NG50 of 59.6 Mbp. 

#### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/bionano/chm13_Saphyr_DLE1.bnx.gz">BNX</a> (md5: 59a7a5583e900e1e5cecb08a34b5b0dc)
   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/bionano/chm13_Saphyr_DLE1.cmap.gz">CMAP</a> (md5: cf1a6fbcf006a26673499b9297664fdb)

## HiC Data

The HiC raw data will be available soon.

## Previously generated PacBio data

The PacBio data was previously generated and is available from the <a href="https://www.ncbi.nlm.nih.gov/sra?linkname=bioproject_sra_all&from_uid=269593">SRA</a>

# Assembly

The current assembly draft (v0.4) is generated with [Canu v1.7.1](https://github.com/marbl/canu) including rel1 data up to 2018/11/15 and incorporating previously released [PacBio](https://www.pacb.com) data. Two gaps on the X plus the centromere were manually resolved. The assembly was polished with two rounds of [nanopolish](https://github.com/jts/nanopolish) and two rounds of [arrow](https://github.com/PacificBiosciences/GenomicConsensus). [BioNano](https://bionanogenomics.com) structural variants on the X were identified, locally mapping nanopore reads selected, reassembled, and used to patch the assembly. However, these patches are not yet polished or validated using BioNano. The assembly has not been curated outside of the X chromosome. The estimated base accuracy is QV36.

The assembly is 2.94 Gbp in size with 657 contigs and an NG50 of 85.8 Mbp

This should be considered a draft and likely has mis-assemblies, inaccurate consensus, and frame-shifted genes. It will be further validated, scaffolded with BioNano, and polished using the available data.

### Downloads

   - <a href="https://s3.amazonaws.com/nanopore-human-wgs/chm13/assemblies/chm13.draft_v0.4.fasta.gz">Assembly draft v0.4</a> (md5: 7e3c2fff9479ba45f7916fa1eee1310b)

# Notes on downloading files.

Files are generously hosted by Amazon Web Services. Although available as straight-forward HTTP links, download performance is improved by using the Amazon Web Services <a href="https://aws.amazon.com/cli/">command-line interface</a>. References should be amended to use the `s3://` addressing scheme, i.e. replace `https://s3.amazon.com/nanopore-human-wgs/` with `s3://nanopore-human-wgs` to download. For example, to download `CHM13_prep5_S13_L002_I1_001.fastq.gz` to the current working directory use the following command.

    aws s3 --no-sign-request cp s3://nanopore-human-wgs/chm13/10x/CHM13_prep5_S13_L002_I1_001.fastq.gz .

or to download the full dataset use the following command.

    aws s3 --no-sign-request sync s3://nanopore-human-wgs/chm13/ .

Amending the `max_concurrent_requests` etc. settings as per <a href="https://docs.aws.amazon.com/cli/latest/topic/s3-config.html">this guide</a> will improve download performance further.

# Contact

Please raise issues on this Github repository concerning this dataset.

# History

    * rel1 and 2: 2nd March 2019. Initial release.
