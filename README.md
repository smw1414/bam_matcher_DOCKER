# Usage
hg19 can be changed to hg38
```shell
docker run --rm  \
-v  /path/to/ucsc.hg19.fa:/genome_files/hg19.fa \
-v  /path/to/ucsc.hg19.fa.fai:/genome_files/hg19.fa.fai \
-v $(pwd):/data \
-v /path/to/bam_folders:/bams \
 hdf87ery/bam_matcher_docker bam-matcher.py -B1 /bams/bam1.bam -B2 \
  /bams/bam2.bam -c /config/bam-matcher.hg19.conf
```
