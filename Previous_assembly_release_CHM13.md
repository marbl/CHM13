# Previous assembly releases of T2T-CHM13

## v2.0 - Latest
 See [Downloads](https://github.com/marbl/CHM13/tree/master?tab=readme-ov-file#downloads).

## v1.1
[Complete T2T reconstruction of a human genome](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v1.1.fasta.gz).
 Changes from v1.0 include filled rDNA gaps and improved polishing within telomeres.
 One rare heterozygous variant causing a premature stop codon was changed at chr9:134589924 to the more common allele.
 Also available at [NCBI GCA_009914755.3](https://www.ncbi.nlm.nih.gov/assembly/GCA_009914755.3).
 Changes made from v1.0 to v1.1 are available as a [VCF](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/changes/v1.0_to_v1.1/v1.0_patch.vcf.gz).

## v1.0
[Complete T2T reconstruction of a human genome](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v1.0.fasta.gz),
 with the exception of 5 known gaps within the rDNA arrays.
 Polished assembly based on v0.9. Introduces 4 structural corrections and 993 small variant corrections, including a 4 kb telomere extension on chr18.
 Polishing was performed using a conservative custom pipeline based on DeepVariant calls and structural corrections were manually curated.
 Consensus quality exceeds Q60. Prior to a preprint being drafted, a brief summary can be found at this [blog post](https://genomeinformatics.github.io/CHM13v1/).
 Also available at [NCBI GCA_009914755.2](https://www.ncbi.nlm.nih.gov/assembly/GCA_009914755.2).
 Changes made from v0.9 to v1.0 are available as a [VCF](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/changes/v0.9_to_v1.0/v0.9_patch.vcf.gz).

## v0.9
[T2T reconstruction of all 23 chromosomes of CHM13](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.9.fasta.gz) based on a custom assembly pipeline, briefly featuring:

1. Homopolymer-compression and self-correction of Pacbio HiFi reads
2. Rescoring of overlaps to account for recurrent Pacbio HiFi errors
3. Construction and custom pruning of a string graph built over 100% identical overlaps
4. Manual reconstruction on chromosomal paths through the graph, if necessary aided by ultra-long Nanopore reads
5. Layout/consensus of original HiFi reads, corresponding to the resulting paths
6. Patching of regions absent from HiFi data with v0.7 draft sequences

Consensus quality exceeds Q60. Mitochondrial sequence DNA included. Centers of the 5 rDNA arrays are represented by N-gaps.

## v0.7
[Assembly draft v0.7](https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.7.fasta.gz) was generated with [Canu v1.7.1](https://github.com/marbl/canu)
 including rel1 data up to 2018/11/15 and incorporating the previously released PacBio data.
 Two gaps on the X plus the centromere were manually resolved. Contigs with low coverage support were split and the assembly was scaffolded with BioNano.
 The assembly was polished with two rounds of [nanopolish](https://github.com/jts/nanopolish) and two rounds of [arrow](https://github.com/PacificBiosciences/GenomicConsensus).
 The X polishing was done using unique markers matched between the assembly and the raw read data, the rest of the genome used traditional polishing.
 Finally, the assembly was polished with 10X Genomics data.
 We [validated](https://github.com/skoren/bacValidation) the assembly using [independent BACs](https://www.ncbi.nlm.nih.gov/nuccore/?term=VMRC59).
 The overall QV is estimated to be Q37 (Q42 in unique regions) and the assembly resolves over 80% of available CHM13 BACs (280/341).
 The assembly is 2.94 Gbp in size with 359 scaffolds (448 contigs) and an NG50 of 83 Mbp (70 Mbp).
 Outside of Chr8 and ChrX, this should be considered a draft and likely has mis-assemblies.
 Older unpolished assemblies are available for benchmarking purposes, but are of lower quality and should not be used for analyses.
 Also available at  [NCBI GCA_009914755.1](https://www.ncbi.nlm.nih.gov/assembly/GCA_009914755.1).

## Downloads
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v1.1.fasta.gz">Assembly draft v1.1</a> (md5: 1cab2b2776005cdf339ec9f283ba2c70)
      - Annotation from <a href="https://github.com/ComparativeGenomicsToolkit/Comparative-Annotation-Toolkit">CAT</a> and <a href="https://github.com/agshumate/Liftoff">Liftoff</a> 
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13.draft_v1.1.gene_annotation.v4.gff3.gz">annotation gff3 file</a> (md5: 14865ece7fe6367b8e2b06776a3d522f)
      - Telomere identified by the <a href="https://github.com/VGP/vgp-assembly/tree/master/pipeline/telomere">VGP</a> pipeline
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13.draft_v1.1.telomere.bed.gz">telomere bed file</a> (md5: d6b148d16bf303e25552e381cddff9df)
      - Liftover from v1.0 to v1.1
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/changes/v1.0_to_v1.1/v1.0_to_v1.1_rdna_merged.chain">chain file</a> (md5: 804d2a81dbf79199fa637f6bbed9a1a8)
      - Liftover from v1.1 to v1.0
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/changes/v1.0_to_v1.1/v1.1_to_v1.0_rdna_merged.chain">chain file</a> (md5: 03180ca0210957e85affc72bb7083b2b)
      - Alignments (the index bai file is available under the same name as the bam with .bai appended (e.g. chm13.draft_v1.1.hifi_20k.wm_2.0.1.pri.bam has a chm13.draft_v1.1.hifi_20k.wm_2.0.1.pri.bam.bai)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.1.hifi_20k.wm_2.01.pri.bam">PacBio HiFi alignments (generated via Winnowmap v2.01 -x map-pb)</a> (md5: ab6b38cb00efa919f6d93bc89787a121)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.1.ont_guppy_3.6.0.wm_2.01.pri.bam">Oxford nanopore Guppy alignments (generated via Winnowmap v2.01 -x map-ont)</a> (md5: 5cb543ac85513995893015a3709806f4)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.1.pcrfree.bam">PCRFree Illumina alignments (generated via bwa mem v0.7.15)</a> (md5: bb41008d0f5de787d26896fb49027420)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v1.0.fasta.gz">Assembly draft v1.0</a> (md5: 6d827b6512562630137008830c46e1ac)
       - Annotation from <a href="https://github.com/ComparativeGenomicsToolkit/Comparative-Annotation-Toolkit">CAT</a> and <a href="https://github.com/agshumate/Liftoff">Liftoff</a> 
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13.draft_v1.0.gene_annotation.v4.gff3.gz">annotation gff3 file</a> (md5: a39f18f553d5a426eaef9cfd4f858bf6)
      - Telomere identified by the <a href="https://github.com/VGP/vgp-assembly/tree/master/pipeline/telomere">VGP</a> pipeline
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13.draft_v1.0.telomere.bed.gz">telomere bed file</a> (md5: 5cdca0c8b563b87f7a624d61ae0b5497)
      - Liftover from hg38 to v1.0 (all files from <a href="https://t2t.gi.ucsc.edu/chm13/hub/t2t-chm13-v1.0/hg38Lastz/">UCSC Genome Browser</a>)
         - <a href="http://t2t.gi.ucsc.edu/chm13/hub/t2t-chm13-v1.0/hg38Lastz/hg38.t2t-chm13-v1.0.over.chain.gz">chain file</a> (md5: ade08feeb01b75644cb1da383ebaa607)
      - Liftover from v1.0 to hg38
         - <a href="http://t2t.gi.ucsc.edu/chm13/hub/t2t-chm13-v1.0/hg38Lastz/t2t-chm13-v1.0.hg38.over.chain.gz">chain file</a> (md5: 9edff5e020cc3f170350ff78fbe01d5c)
      - Alignments (the index bai file is available under the same name as the bam with .bai appended (e.g. chm13.draft_v1.0.wm_2.01.hifi.pri.bam has a chm13.draft_v1.0.wm_2.01.hifi.pri.bam.bai)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.0.clr_p6c4.wm_2.01.pri.bam">PacBio CLR alignments (generated via Winnowmap v2.01 -x map-pb-clr)</a> (md5: 235e23c72676279714a091fb226f3b1a)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.0.hifi_20k.wm_2.01.pri.bam">PacBio HiFi alignments (generated via Winnowmap v2.01 -x map-pb)</a> (md5: 2380bee4c3544d179b51cf22846e33ab)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.0.ont_guppy_3.6.0.wm_2.01.pri.bam">Oxford nanopore Guppy alignments (generated via Winnowmap v2.01 -x map-ont)</a> (md5: 5a012ae791f48678b829da6770216f5d)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.0.ont_bonito_0.3.1.wm_2.01.pri.bam">Oxford nanopore Bonito alignments (generated via Winnowmap v2.01 -x map-ont)</a> (md5: 84b0b9d5935140ead1d032b0a1610c39)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v1.0.pcrfree.bam">PCRFree Illumina alignments (generated via bwa mem v0.7.15)</a> (md5: 9143c6d6dc3e8f537c49f43f9e6cbedd)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.9.fasta.gz">Assembly draft v0.9</a> (md5: 05fd40ffc5d68a9b6754773a56381db8)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/annotation/chm13.draft_v0.9.region.bed.gz">Regions patched by non-HiFi data & rDNA loci</a> (md5: a754f98d5e960b3d1e9029cba4414cf2)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/graph/chm13.draft_v0.9.simplified.compress.gfa.gz">v0.9 assembly graph in GFA format (built over homopolymer-compressed HiFi reads)</a> (md5: df2218db9ebbcd239d07d2544372cfa5)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/graph/chm13.draft_v0.9.simplified.nodes.fasta.gz">Consensus sequences for individual nodes of the v0.9 assembly graph (since the sequence is not homopolymer compressed, the lengths and overlap sizes will not match the GFA!)</a> (md5: 086d3d968b2c8cbc8c4be891e56ad177)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/graph/chm13.draft_v0.9.layouts.tgz">Genomic paths through the v0.9 graph (part of chr9 was reconstructed by a different assembly method excluded)</a> (md5: 913205d75f5f9c49e5269eb4363fbf16)
      - Alignments (the index bai file is available under the same name as the bam with .bai appended (e.g. chm13.draft_v0.9.clr.bam has a chm13.draft_v0.9.clr.bam.bai)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v0.9.clr.bam">PacBio CLR alignments (generated via Winnowmap v1.11 -x map-pb-clr)</a> (md5: 7cd9c812e4398db6ed318969fe7080f9)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v0.9.hifi.bam">PacBio HiFi alignments (generated via Winnowmap v1.11 -x map-pb)</a> (md5: 7527b44aba07d9acbed597fbc445b61a)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v0.9.ont.bam">Oxford nanopore alignments (generated via Winnowmap v1.11 -x map-ont)</a> (md5: 4a5bbf70193e65c35a287a70099bb99c)
         - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.draft_v0.9.pcrfree.bam">PCRFree Illumina alignments (generated via bwa mem v0.7.15)</a> (md5: 7c13fd36ae404eb41697ec5d54ba608f)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.chrX_v0.7.fasta.gz">Chromosome X v0.7</a> (md5: 89b3dd61db66177dd830527b920956fa)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/nanopore/rel1/rel1_to_v0.7_chrX.filtered.bam">Chromosome X v0.7 Nanopore rel1 unique k-mer anchored mappings</a> (md5: ada12a00d4781f6b0101a09be19abe93)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.chrX_v0.7.pacbioHiFi.bam">Chromosome X v0.7 PacBio HiFi unique k-mer anchored mappings</a> (md5: bd22daaf6d4a2cd775f109a853a911a9)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/alignments/chm13.chrX_v0.7.pacbioCLR.bam">Chromosome X v0.7 PacBio CLR unique k-mer anchored mappings</a> (md5: 69be7bd105ee590bf57853c249e1f8d8)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.chr8_v9.fasta.gz">Chromosome 8 v9</a> (md5: cc33037728ab1f743d3e79f85e8c10ac)
      - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/nanopore/rel5/rel5_to_chr8_v9.filtered.bam">Chromosome 8 v9 Nanopore rel5 unique k-mer anchored mappings</a> (md5: e953525b097c98d8485a3a7b152da897)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.7.fasta.gz">Assembly draft v0.7</a> (md5: b9777540aaa0251c7dbb4974fb0a69d6)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.6.fasta.gz">Assembly draft v0.6</a> (md5: c3e3318e82ba5dc64b74f458f4989b85)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/CHM13/assemblies/chm13.draft_v0.4.fasta.gz">Assembly draft v0.4</a> (md5: 7e3c2fff9479ba45f7916fa1eee1310b)
   - <a href="https://s3-us-west-2.amazonaws.com/human-pangenomics/T2T/HG002/assemblies/HG002.chrX_v0.7.fasta.gz">HG002 chrX draft v0.7 (not T2T, missing p-arm PAR region)</a> (md5: 1d79ac022424fc5671135e2ac362d91d)

