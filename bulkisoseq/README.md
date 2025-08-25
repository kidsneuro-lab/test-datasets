# Files

- [bulkisoseq/data/samplesheet.csv](bulkisoseq/data/samplesheet.csv)
- [bulkisoseq/data/111_TEST_P_C.bam](bulkisoseq/data/111_TEST_P_C.bam)
- [bulkisoseq/data/222_TEST_P_C.bam](bulkisoseq/data/222_TEST_P_C.bam)


# Samples

| sample       | source                                                                                                                                                           |
|--------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 111_TEST_P_C.bam | https://downloads.pacbcloud.com/public/dataset/Kinnex-full-length-RNA/DATA-Revio-SCRI-Sample3-Heart-Control/0-CCS/m84039_230627_232423_s4.hifi_reads.bcM0003.bam |
| 222_TEST_P_C.bam | https://downloads.pacbcloud.com/public/dataset/Kinnex-full-length-RNA/DATA-Revio-SCRI-Sample6-Cerebellum/0-CCS/m84039_230628_230337_s3.hifi_reads.bcM0002.bam |

**Generating the samples**

111_TEST_P_C.bam
```bash
samtools view -b --subsample 0.00101725260416666667 --subsample-seed 1 -o 111_TEST_P_C.bam https://downloads.pacbcloud.com/public/dataset/Kinnex-full-length-RNA/DATA-Revio-SCRI-Sample3-Heart-Control/0-CCS/m84039_230627_232423_s4.hifi_reads.bcM0003.bam
```

```bash
samtools view -b --subsample 0.00085663377192982456 --subsample-seed 1 -o 222_TEST_P_C.bam https://downloads.pacbcloud.com/public/dataset/Kinnex-full-length-RNA/DATA-Revio-SCRI-Sample6-Cerebellum/0-CCS/m84039_230628_230337_s3.hifi_reads.bcM0002.bam
```

# Samtools version
```bash
$ samtools version
samtools 1.22.1
Using htslib 1.22.1
```