
################## Notes updated on March 13, 2017 by Qianyi
The rat F1 contain 10 samples, 53317 - 53326. 
The initial number of total reads for each sample varies from 43 million to 82 million. 
The paired reads have read length of 126 and %GC of 47-50. QC was performed using FastQC. 

These 10 samples were aligned to July 2014 assembly of Rattus norvegicus genome (RGSC Rnor_6.0, UCSC version rn6) 
using STAR v2.5.1a with the following command:
$STAR --genomeDir ${genomedir} --runThreadN 5 --readFilesIn ${read1} ${read2} --readFilesCommand zcat --sjdbGTFfile ${gtf} --outFileNamePrefix ${outdir}/${prefix}star1. --outFilterMatchNminOverLread 0.4 --outFilterScoreMinOverLread 0.4
For each sample, there were 88%-91% uniquely mapped reads.
#####################################################
