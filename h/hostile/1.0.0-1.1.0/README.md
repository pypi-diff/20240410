# Comparing `tmp/hostile-1.0.0.tar.gz` & `tmp/hostile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hostile-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "hostile-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `hostile-1.0.0.tar` & `hostile-1.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0      715 2023-07-10 14:24:39.989614 hostile-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1840 2023-07-10 14:19:21.498360 hostile-1.0.0/.gitignore
--rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      676 2023-08-31 11:06:09.926890 hostile-1.0.0/Dockerfile
--rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-1.0.0/LICENSE
--rw-r--r--   0        0        0    13502 2024-01-22 18:01:35.709237 hostile-1.0.0/README.md
--rw-r--r--   0        0        0     2068 2024-01-22 16:19:20.955436 hostile-1.0.0/bucket/manifest.json
--rw-r--r--   0        0        0      198 2023-11-22 16:45:11.889058 hostile-1.0.0/environment.yml
--rw-r--r--   0        0        0   951199 2023-08-02 18:00:37.538126 hostile-1.0.0/logo.png
--rw-r--r--   0        0        0   229015 2024-01-14 22:04:28.033239 hostile-1.0.0/paper/article.pdf
--rw-r--r--   0        0        0     7171 2023-11-22 16:45:08.409696 hostile-1.0.0/paper/supplementary-table-1.tsv
--rw-r--r--   0        0        0    11491 2023-07-20 18:21:17.921904 hostile-1.0.0/paper/supplementary-table-2.tsv
--rw-r--r--   0        0        0   122195 2023-08-22 10:59:46.622412 hostile-1.0.0/paper/supplementary-table-3.tsv
--rw-r--r--   0        0        0   264713 2023-11-11 20:18:28.358650 hostile-1.0.0/paper/supplementary-table-4.tsv
--rw-r--r--   0        0        0   113361 2023-11-11 22:27:14.521809 hostile-1.0.0/paper/supplementary-text.pdf
--rw-r--r--   0        0        0      679 2024-01-22 13:36:45.675910 hostile-1.0.0/pyproject.toml
--rw-r--r--   0        0        0   208844 2023-08-24 15:38:46.365367 hostile-1.0.0/screenshot.png
--rw-r--r--   0        0        0       55 2024-01-20 14:55:00.535853 hostile-1.0.0/src/hostile/__init__.py
--rw-r--r--   0        0        0    11250 2024-01-22 18:11:04.485380 hostile-1.0.0/src/hostile/aligner.py
--rw-r--r--   0        0        0     5941 2024-01-22 18:25:06.224784 hostile-1.0.0/src/hostile/cli.py
--rw-r--r--   0        0        0    11493 2024-01-22 18:20:48.182181 hostile-1.0.0/src/hostile/lib.py
--rw-r--r--   0        0        0     6606 2024-01-22 11:34:00.883154 hostile-1.0.0/src/hostile/util.py
--rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 hostile-1.0.0/tests/data/human_1_1.fastq.gz
--rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 hostile-1.0.0/tests/data/human_1_2.fastq.gz
--rw-r--r--   0        0        0   180149 2024-01-10 20:07:33.437904 hostile-1.0.0/tests/data/mask/gallid-herpesvirus-2.fa
--rw-r--r--   0        0        0     2535 2024-01-10 20:07:33.438320 hostile-1.0.0/tests/data/mask/t2t-chm13v2.0-chr21-subset.fa
--rw-r--r--   0        0        0      811 2023-07-10 11:24:36.269899 hostile-1.0.0/tests/data/sars-cov-2/partial-for-mask-testing.fa.gz
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.2.bt2
--rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.3.bt2
--rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.4.bt2
--rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.fasta.gz
--rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.rev.1.bt2
--rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.rev.2.bt2
--rw-r--r--   0        0        0     4104 2023-07-23 10:44:52.122889 hostile-1.0.0/tests/data/sars-cov-2_100_1.fastq.gz
--rw-r--r--   0        0        0     4263 2023-07-23 10:44:58.804478 hostile-1.0.0/tests/data/sars-cov-2_100_2.fastq.gz
--rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874003 hostile-1.0.0/tests/data/sars-cov-2_1_1.fastq
--rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874201 hostile-1.0.0/tests/data/sars-cov-2_1_2.fastq
--rw-r--r--   0        0        0     2249 2024-01-21 11:53:50.160661 hostile-1.0.0/tests/data/sars-cov-2_50_2.fastq.gz
--rw-r--r--   0        0        0      335 2023-07-06 18:18:11.925871 hostile-1.0.0/tests/data/tuberculosis_1_1.fastq
--rw-r--r--   0        0        0      239 2023-07-06 18:18:11.925871 hostile-1.0.0/tests/data/tuberculosis_1_1.fastq.gz
--rw-r--r--   0        0        0      335 2023-07-06 18:18:11.926049 hostile-1.0.0/tests/data/tuberculosis_1_2.fastq
--rw-r--r--   0        0        0      232 2023-07-06 18:18:11.926049 hostile-1.0.0/tests/data/tuberculosis_1_2.fastq.gz
--rw-r--r--   0        0        0      668 2023-11-10 14:20:16.446185 hostile-1.0.0/tests/data/tuberculosis_2.fastq
--rw-r--r--   0        0        0    21700 2024-01-22 17:14:47.007666 hostile-1.0.0/tests/test_all.py
--rw-r--r--   0        0        0    14112 1970-01-01 00:00:00.000000 hostile-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      715 2023-07-10 14:24:39.989614 hostile-1.1.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1840 2023-07-10 14:19:21.498360 hostile-1.1.0/.gitignore
+-rw-r--r--   0        0        0      260 2023-05-31 15:56:25.388315 hostile-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      619 2024-04-10 20:57:15.994448 hostile-1.1.0/Dockerfile
+-rw-r--r--   0        0        0     1086 2023-05-23 13:13:09.919197 hostile-1.1.0/LICENSE
+-rw-r--r--   0        0        0    14602 2024-04-10 21:08:10.605576 hostile-1.1.0/README.md
+-rw-r--r--   0        0        0     2068 2024-01-22 16:19:20.955436 hostile-1.1.0/bucket/manifest.json
+-rw-r--r--   0        0        0      198 2024-01-22 19:29:58.757198 hostile-1.1.0/environment.yml
+-rw-r--r--   0        0        0   951199 2023-08-02 18:00:37.538126 hostile-1.1.0/logo.png
+-rw-r--r--   0        0        0   229015 2024-01-14 22:04:28.033239 hostile-1.1.0/paper/article.pdf
+-rw-r--r--   0        0        0     7171 2023-11-22 16:45:08.409696 hostile-1.1.0/paper/supplementary-table-1.tsv
+-rw-r--r--   0        0        0    11491 2023-07-20 18:21:17.921904 hostile-1.1.0/paper/supplementary-table-2.tsv
+-rw-r--r--   0        0        0   122195 2023-08-22 10:59:46.622412 hostile-1.1.0/paper/supplementary-table-3.tsv
+-rw-r--r--   0        0        0   264713 2023-11-11 20:18:28.358650 hostile-1.1.0/paper/supplementary-table-4.tsv
+-rw-r--r--   0        0        0   113361 2023-11-11 22:27:14.521809 hostile-1.1.0/paper/supplementary-text.pdf
+-rw-r--r--   0        0        0      679 2024-01-22 13:36:45.675910 hostile-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0   208844 2023-08-24 15:38:46.365367 hostile-1.1.0/screenshot.png
+-rw-r--r--   0        0        0       55 2024-04-10 21:13:26.129371 hostile-1.1.0/src/hostile/__init__.py
+-rw-r--r--   0        0        0    11223 2024-03-05 20:16:57.438911 hostile-1.1.0/src/hostile/aligner.py
+-rw-r--r--   0        0        0     6071 2024-03-05 20:16:57.439108 hostile-1.1.0/src/hostile/cli.py
+-rw-r--r--   0        0        0    11121 2024-01-29 20:57:36.641718 hostile-1.1.0/src/hostile/lib.py
+-rw-r--r--   0        0        0     6980 2024-04-10 13:20:03.976417 hostile-1.1.0/src/hostile/util.py
+-rw-r--r--   0        0        0      164 2023-07-06 18:18:11.924762 hostile-1.1.0/tests/data/human_1_1.fastq.gz
+-rw-r--r--   0        0        0      178 2023-07-06 18:18:11.925005 hostile-1.1.0/tests/data/human_1_2.fastq.gz
+-rw-r--r--   0        0        0   180149 2024-01-10 20:07:33.437904 hostile-1.1.0/tests/data/mask/gallid-herpesvirus-2.fa
+-rw-r--r--   0        0        0     2535 2024-01-10 20:07:33.438320 hostile-1.1.0/tests/data/mask/t2t-chm13v2.0-chr21-subset.fa
+-rw-r--r--   0        0        0      811 2023-07-10 11:24:36.269899 hostile-1.1.0/tests/data/sars-cov-2/partial-for-mask-testing.fa.gz
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.881250 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.881240 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.2.bt2
+-rw-r--r--   0        0        0       17 2023-06-02 16:28:46.850838 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.3.bt2
+-rw-r--r--   0        0        0     7476 2023-06-02 16:28:46.850709 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.4.bt2
+-rw-r--r--   0        0        0     9458 2022-07-08 10:03:05.588963 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.fasta.gz
+-rw-r--r--   0        0        0  4204460 2023-06-02 16:28:46.913064 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.rev.1.bt2
+-rw-r--r--   0        0        0     7480 2023-06-02 16:28:46.913055 hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.rev.2.bt2
+-rw-r--r--   0        0        0     4104 2023-07-23 10:44:52.122889 hostile-1.1.0/tests/data/sars-cov-2_100_1.fastq.gz
+-rw-r--r--   0        0        0     4263 2023-07-23 10:44:58.804478 hostile-1.1.0/tests/data/sars-cov-2_100_2.fastq.gz
+-rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874003 hostile-1.1.0/tests/data/sars-cov-2_1_1.fastq
+-rw-r--r--   0        0        0      319 2023-07-23 12:01:36.874201 hostile-1.1.0/tests/data/sars-cov-2_1_2.fastq
+-rw-r--r--   0        0        0     2249 2024-01-21 11:53:50.160661 hostile-1.1.0/tests/data/sars-cov-2_50_2.fastq.gz
+-rw-r--r--   0        0        0      335 2023-07-06 18:18:11.925871 hostile-1.1.0/tests/data/tuberculosis_1_1.fastq
+-rw-r--r--   0        0        0      239 2023-07-06 18:18:11.925871 hostile-1.1.0/tests/data/tuberculosis_1_1.fastq.gz
+-rw-r--r--   0        0        0      335 2023-07-06 18:18:11.926049 hostile-1.1.0/tests/data/tuberculosis_1_2.fastq
+-rw-r--r--   0        0        0      232 2023-07-06 18:18:11.926049 hostile-1.1.0/tests/data/tuberculosis_1_2.fastq.gz
+-rw-r--r--   0        0        0      668 2023-11-10 14:20:16.446185 hostile-1.1.0/tests/data/tuberculosis_2.fastq
+-rw-r--r--   0        0        0    21700 2024-02-29 13:37:39.919044 hostile-1.1.0/tests/test_all.py
+-rw-r--r--   0        0        0    15212 1970-01-01 00:00:00.000000 hostile-1.1.0/PKG-INFO
```

### Comparing `hostile-1.0.0/.github/workflows/test.yml` & `hostile-1.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/.gitignore` & `hostile-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/Dockerfile` & `hostile-1.1.0/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Bioconda-based build against main branch
 FROM condaforge/miniforge3:latest
 RUN git clone https://github.com/bede/hostile.git
-RUN sed -i 's/name: hostile/name: base/' hostile/environment.yml
-RUN mamba env update -f hostile/environment.yml
+RUN mamba env update -n base -f hostile/environment.yml
 RUN pip install ./hostile[dev]
 RUN cd hostile && pytest
 
 ## Debian-based build against main branch
 # FROM ubuntu:22.04
 # RUN apt-get update && apt-get -y install bowtie2 minimap2 bedtools samtools python3-pip git
 # RUN git clone https://github.com/bede/hostile.git
```

### Comparing `hostile-1.0.0/LICENSE` & `hostile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/README.md` & `hostile-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 <p align="center">
     <img width="250" src="logo.png">
 </p>
 
 # Hostile
 
-Hostile accurately removes host sequences from short and long read (meta)genomes, consuming paired or unpaired `fastq[.gz]` input. Batteries are included – a human reference genome is downloaded when run for the first time. Hostile is precise by default, removing an [order of magnitude fewer microbial reads](https://log.bede.im/2023/08/29/precise-host-read-removal.html#evaluating-accuracy) than existing approaches while removing >99.5% of real human reads from 1000 Genomes Project samples. For the best possible retention of microbial reads, use an existing index masked against bacterial and/or viral genomes, or make your own using the built-in masking utility. Read headers can be replaced with integers (using `--rename`) for privacy and smaller FASTQs. Heavy lifting is done with fast existing tools (Minimap2/Bowtie2 and Samtools). Bowtie2 is the default aligner for short (paired) reads while Minimap2 is default aligner for long reads. In benchmarks, bacterial Illumina reads were decontaminated at 32Mbp/s (210k reads/sec) and bacterial ONT reads at 22Mbp/s, using 8 alignment threads. Further information and benchmarks can be found in the [paper](https://doi.org/10.1093/bioinformatics/btad728) and [blog post](https://log.bede.im/2023/08/29/precise-host-read-removal.html). Please open an issue to report problems [or](mailto:b@bede.im) [otherwise](https://twitter.com/beconsta) [reach](https://bsky.app/profile/bedec.bsky.social) [out](https://mstdn.science/@bede) for help, advice etc.
+Hostile accurately removes host sequences from short and long read (meta)genomes, consuming paired or unpaired `fastq[.gz]` input. Batteries are included – a human reference genome is downloaded when run for the first time. Hostile is precise by default, removing an [order of magnitude fewer microbial reads](https://log.bede.im/2023/08/29/precise-host-read-removal.html#evaluating-accuracy) than existing approaches while removing >99.5% of real human reads from 1000 Genomes Project samples. For the best possible retention of microbial reads, use an existing index masked against bacterial and/or viral genomes, or make your own using the built-in masking utility. Read headers can be replaced with integers (using `--rename`) for privacy and smaller FASTQs. Heavy lifting is done with fast existing tools (Minimap2/Bowtie2 and Samtools). Bowtie2 is the default aligner for short (paired) reads while Minimap2 is default aligner for long reads. In benchmarks, bacterial Illumina reads were decontaminated at 32Mbp/s (210k reads/sec) and bacterial ONT reads at 22Mbp/s, using 8 alignment threads. By default, Hostile requires 4GB of RAM for decontaminating short reads and 13GB for long reads (Minimap2). Further information and benchmarks can be found in the [paper](https://doi.org/10.1093/bioinformatics/btad728) and [blog post](https://log.bede.im/2023/08/29/precise-host-read-removal.html). Please open an issue to report problems [or](mailto:b@bede.im) [otherwise](https://twitter.com/beconsta) [reach](https://bsky.app/profile/bedec.bsky.social) [out](https://mstdn.science/@bede) for help, advice etc.
 
 
 
 ## Reference genomes (indexes)
 
-The default index `human-t2t-hla` comprises [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) and [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51, and is downloaded automatically when running Hostile unless another index is specified. Slightly higher microbial sequence retention is possible using a masked index, of which several are available. The index `human-t2t-hla-argos985` is masked against [985 reference grade bacterial genomes](https://www.ncbi.nlm.nih.gov/bioproject/231221) including common human pathogens, while `human-t2t-hla-argos985-mycob140` is further masked against mycobacterial genomes. To use a standard index, simply pass its name as the value of the `--index` argument which takes care of downloading and cacheing the relevant index. Automatic download can be disabled using the `--offline` flag, and `--index` can accept a path to a custom reference genome or Bowtie2 index. [Object storage](https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o) is provided by the [ModMedMicro research group](https://www.expmedndm.ox.ac.uk/modernising-medical-microbiology).
+The default index `human-t2t-hla` comprises [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) and [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51, and is downloaded automatically when running Hostile unless another index is specified. Slightly higher microbial sequence retention is may be possible using masked indexes, listed below. The index `human-t2t-hla-argos985` is masked against [985 reference grade bacterial genomes](https://www.ncbi.nlm.nih.gov/bioproject/231221) including common human pathogens, while `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` is further masked comoprehensively against all known virus and phage genomes. The latter should be used when retention of viral sequences is a priority. To use a standard index, simply pass its name as the value of the `--index` argument which takes care of downloading and caching the relevant index. Automatic download can be disabled using the `--offline` flag, and `--index` can accept a path to a custom reference genome or Bowtie2 index. [Object storage](https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o) is provided by the [ModMedMicro research unit](https://www.expmedndm.ox.ac.uk/modernising-medical-microbiology) at the University of Oxford.
 
 |                             Name                             |                         Composition                          | Date    | Masked positions       |
 | :----------------------------------------------------------: | :----------------------------------------------------------: | ------- | ---------------------- |
 |                `human-t2t-hla` **(default)**                 | [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) + [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51 | 2023-07 | 0 (**0%**)             |
 |                   `human-t2t-hla-argos985`                   | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial** genomes | 2023-07 | 317,973 (**0.010%**)   |
 |       `human-t2t-hla.rs-viral-202401_ml-phage-202401`        | `human-t2t-hla` masked with 150mers for 18,719 RefSeq **viral** and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,172,993 (**0.037%**) |
-| `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) bacterial, 18,719 RefSeq **viral**, and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,473,260 (**0.046%**) |
+| `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial**, 18,719 RefSeq **viral**, and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,473,260 (**0.046%**) |
 |              `human-t2t-hla-argos985-mycob140`               | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial** & [140](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) **mycobacterial** genomes | 2023-07 | 319,752 (**0.010%**)   |
 
 *Performance of `human-t2t-hla` and `human-t2t-hla-argos985-mycob140` was evaluated in the [paper](https://doi.org/10.1093/bioinformatics/btad728)*
 
 
 
 ## Install  [![Install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat-square&logo=anaconda)](https://biocontainers.pro/tools/hostile) [![Install with Docker](https://img.shields.io/badge/install%20with-docker-important.svg?style=flat-square&logo=docker)](https://biocontainers.pro/tools/hostile)
@@ -36,52 +36,53 @@
 conda create -y -n hostile -c conda-forge -c bioconda hostile
 conda activate hostile
 ```
 
 **Docker**
 
 ```bash
-docker run quay.io/biocontainers/hostile:0.4.0--pyhdfd78af_0
-
-# Build your own
 wget https://raw.githubusercontent.com/bede/hostile/main/Dockerfile
 docker build . --platform linux/amd64
 ```
 
+A [Biocontainer image](https://biocontainers.pro/tools/hostile) is also available, but beware that this often lags behind the latest released version
+
 
 
 ## Index installation (optional)
 
 Hostile automatically downloads and caches the default index `human-t2t-hla` when run for the first time, meaning that there is no need to download an index in advance. Neverthless:
 
 - To download and cache the default index (`human-t2t-hla`), run `hostile fetch`
 - To list available indexes, run `hostile fetch --list`
 - To download and cache another standard index, run e.g. `hostile fetch --name human-t2t-hla-argos985`
-- To use a custom genome (made perhaps with `hostile mask`), run `hostile clean --index path/to/genome.fa`
+- To use a custom genome (made with e.g. `hostile mask`), run `hostile clean` with  `--index path/to/genome.fa` (minimap2) or `--index path/to/index` (without file extensions; Bowtie2)
+- To change where indexes are stored, set the environment variable `HOSTILE_CACHE_DIR` to a directory of your choice. Run `hostile fetch --list` to verify.
 
 
 
 ## Command line usage
 
 ```bash
 $ hostile clean -h
-usage: hostile clean [-h] --fastq1 FASTQ1 [--fastq2 FASTQ2] [--aligner {bowtie2,minimap2,auto}] [--index INDEX] [--invert] [--rename] [--reorder] [--out-dir OUT_DIR] [--threads THREADS] [--aligner-args ALIGNER_ARGS] [--force]
-                     [--offline] [--debug]
+usage: hostile clean [-h] --fastq1 FASTQ1 [--fastq2 FASTQ2] [--aligner {bowtie2,minimap2,auto}] [--index INDEX]
+                     [--invert] [--rename] [--reorder] [--out-dir OUT_DIR] [--threads THREADS]
+                     [--aligner-args ALIGNER_ARGS] [--force] [--offline] [--debug]
 
-Remove reads aligning to a target genome from fastq[.gz] input files.
+Remove reads aligning to an index from fastq[.gz] input files
 
 options:
   -h, --help            show this help message and exit
   --fastq1 FASTQ1       path to forward fastq[.gz] file
   --fastq2 FASTQ2       optional path to reverse fastq[.gz] file
                         (default: None)
   --aligner {bowtie2,minimap2,auto}
                         alignment algorithm. Default is Bowtie2 (paired reads) & Minimap2 (unpaired reads)
                         (default: auto)
-  --index INDEX         name of standard index or path to custom index
+  --index INDEX         name of standard index or path to custom genome/index
                         (default: human-t2t-hla)
   --invert              keep only reads aligning to the target genome (and their mates if applicable)
                         (default: False)
   --rename              replace read names with incrementing integers
                         (default: False)
   --reorder             ensure deterministic output order
                         (default: False)
@@ -102,16 +103,16 @@
 
 
 
 **Short reads, default index**
 
 ```bash
 $ hostile clean --fastq1 human_1_1.fastq.gz --fastq2 human_1_2.fastq.gz
-INFO: Hostile version 1.0.0. Using Bowtie2 (paired reads)
-INFO: Found cached standard index human-t2t-hla (Bowtie2)
+INFO: Hostile version 1.0.0. Mode: paired short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 [
     {
         "version": "1.0.0",
         "aligner": "bowtie2",
         "index": "human-t2t-hla",
@@ -127,32 +128,48 @@
         "fastq2_in_name": "human_1_2.fastq.gz",
         "fastq2_in_path": "/Users/bede/human_1_2.fastq.gz",
         "fastq2_out_name": "human_1_2.clean_2.fastq.gz",
         "fastq2_out_path": "/Users/bede/human_1_2.clean_2.fastq.gz"
     }
 ]
 ```
+
+
 **Short reads, masked index, save log**
 
 ```bash
 $ hostile clean --fastq1 human_1_1.fastq.gz --fastq2 human_1_2.fastq.gz --index human-t2t-hla-argos985 > log.json
-INFO: Hostile version 1.0.0. Using Bowtie2 (paired reads)
-INFO: Found cached standard index human-t2t-hla (Bowtie2)
+INFO: Hostile version 1.0.0. Mode: paired short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
+INFO: Cleaning…
+INFO: Cleaning complete
+```
+
+
+
+**Short unpaired reads, save log**
+
+By default, single fastqs are assumed to be long reads. Override this by specifying `--aligner bowtie2` when decontaminating unpaired short reads.
+
+```bash
+$ hostile clean --aligner bowtie2 --fastq1 tests/data/human_1_1.fastq.gz > log.json
+INFO: Hostile version 1.0.0. Mode: short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 ```
 
 
 
 **Long reads**
 
 ```bash
 $ hostile clean --fastq1 tests/data/tuberculosis_1_1.fastq.gz
-INFO: Hostile version 1.0.0. Using Minimap2's long read preset
-INFO: Found cached standard index human-t2t-hla (Minimap2)
+INFO: Hostile version 1.0.0. Mode: long read (Minimap2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 [
     {
         "version": "1.0.0",
         "aligner": "minimap2",
         "index": "human-t2t-hla",
@@ -204,17 +221,18 @@
 ```bash
 hostile mask human.fasta lots-of-bacterial-genomes.fasta --threads 8
 ```
 You may wish to use one of the existing [reference genomes](#reference-genomes--indexes) as a starting point. Masking uses Minimap2 to align 150mers of the supplied target genomes with the reference genome, and bedtools to mask all aligned regions with N. Both a masked genome (for Minimap2) and a masked Bowtie2 index is created.
 
 
 
-## Known issues
+## Limitations
 
-- Using more than 10 alignment threads may reduce performance, even on systems with enough CPU cores. A sensible default is therefore chosen automatically at runtime. To maximise performance on your system, some experimentation may be necessary.
+- Hostile prioritises retaining microbial sequences above discarding host sequences. If you strive to remove every last human sequence, other approaches may serve you better.
+- Performance is not always improved by using all available CPU cores. A sensible default is therefore chosen automatically at runtime based on the number of available CPU cores.
 - Minimap2 has an overhead of 30-90s for human genome indexing prior to starting decontamination. Surprisingly, loading a prebuilt index is not significantly faster. I hope to mitigate this in a future release.
 
 
 
 ## Citation
 
 Bede Constantinides, Martin Hunt, Derrick W Crook,  Hostile: accurate decontamination of microbial host sequences, *Bioinformatics*, 2023; btad728, https://doi.org/10.1093/bioinformatics/btad728
```

### Comparing `hostile-1.0.0/bucket/manifest.json` & `hostile-1.1.0/bucket/manifest.json`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/logo.png` & `hostile-1.1.0/logo.png`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/article.pdf` & `hostile-1.1.0/paper/article.pdf`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/supplementary-table-1.tsv` & `hostile-1.1.0/paper/supplementary-table-1.tsv`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/supplementary-table-2.tsv` & `hostile-1.1.0/paper/supplementary-table-2.tsv`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/supplementary-table-3.tsv` & `hostile-1.1.0/paper/supplementary-table-3.tsv`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/supplementary-table-4.tsv` & `hostile-1.1.0/paper/supplementary-table-4.tsv`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/paper/supplementary-text.pdf` & `hostile-1.1.0/paper/supplementary-text.pdf`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/pyproject.toml` & `hostile-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/screenshot.png` & `hostile-1.1.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/src/hostile/aligner.py` & `hostile-1.1.0/src/hostile/aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             raise RuntimeError(f"Failed to execute {self.bin_path}")
         if self.name == "Bowtie2":
             if Path(f"{index}.1.bt2").is_file():
                 index_path = Path(index)
                 logging.info(f"Found custom index {index_path}")
             elif (self.data_dir / f"{index}.1.bt2").is_file():
                 index_path = self.data_dir / index
-                logging.info(f"Found cached standard index {index} (Bowtie2)")
+                logging.info(f"Found cached standard index {index}")
             elif not offline and util.fetch_manifest(util.BUCKET_URL).get(index):
                 file_name = f"{index}.tar"
                 file_url = f"{util.BUCKET_URL}/{file_name}"
                 logging.info(f"Fetching standard index {index} ({file_url})")
                 manifest = util.fetch_manifest(util.BUCKET_URL)
                 with tempfile.NamedTemporaryFile() as temporary_file:
                     tmp_path = Path(temporary_file.name)
@@ -61,15 +61,15 @@
                 raise FileNotFoundError(message)
         elif self.name == "Minimap2":
             if Path(f"{index}").is_file():
                 index_path = Path(index)
                 logging.info(f"Found custom index {index}")
             elif (self.data_dir / f"{index}.fa.gz").is_file():
                 index_path = self.data_dir / f"{index}.fa.gz"
-                logging.info(f"Found cached standard index {index} (Minimap2)")
+                logging.info(f"Found cached standard index {index}")
             elif not offline and util.fetch_manifest(util.BUCKET_URL).get(index):
                 file_name = f"{index}.fa.gz"
                 file_url = f"{util.BUCKET_URL}/{file_name}"
                 logging.info(f"Fetching standard index {index} ({file_url})")
                 manifest = util.fetch_manifest(util.BUCKET_URL)
                 with tempfile.NamedTemporaryFile() as temporary_file:
                     tmp_path = Path(temporary_file.name)
@@ -230,27 +230,27 @@
 ALIGNER = Enum(
     "Aligner",
     {
         "bowtie2": Aligner(
             name="Bowtie2",
             short_name="bt2",
             bin_path=Path("bowtie2"),
-            data_dir=util.XDG_DATA_DIR,
+            data_dir=util.CACHE_DIR,
             cmd=(
                 "{BIN_PATH} -x '{INDEX_PATH}' -U '{FASTQ}'"
                 " -k 1 --mm -p {THREADS} {ALIGNER_ARGS}"
             ),
             paired_cmd=(
                 "{BIN_PATH} -x '{INDEX_PATH}' -1 '{FASTQ1}' -2 '{FASTQ2}'"
                 " -k 1 --mm -p {THREADS} {ALIGNER_ARGS}"
             ),
         ),
         "minimap2": Aligner(
             name="Minimap2",
             short_name="mm2",
             bin_path=Path("minimap2"),
-            data_dir=util.XDG_DATA_DIR,
+            data_dir=util.CACHE_DIR,
             cmd="{BIN_PATH} -ax map-ont -m 40 --secondary no -t {THREADS} {ALIGNER_ARGS} '{INDEX_PATH}' '{FASTQ}'",
             paired_cmd="{BIN_PATH} -ax sr -m 40 --secondary no -t {THREADS} {ALIGNER_ARGS} '{INDEX_PATH}' '{FASTQ1}' '{FASTQ2}'",
         ),
     },
 )
```

### Comparing `hostile-1.0.0/src/hostile/cli.py` & `hostile-1.1.0/src/hostile/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def clean(
     *,
     fastq1: Path,
     fastq2: Path | None = None,
     aligner: ALIGNER = ALIGNER.auto,
-    index: str = "human-t2t-hla",
+    index: str = util.DEFAULT_INDEX_NAME,
     invert: bool = False,
     rename: bool = False,
     reorder: bool = False,
     out_dir: Path = util.CWD,
     threads: int = util.THREADS,
     aligner_args: str = "",
     force: bool = False,
@@ -120,35 +120,37 @@
         kmer_length=kmer_length,
         kmer_step=kmer_step,
         threads=threads,
     )
 
 
 def fetch(
-    name: str = "human-t2t-hla",
+    name: str = util.DEFAULT_INDEX_NAME,
     aligner: Literal["minimap2", "bowtie2", "both"] = "both",
     list: bool = False,
 ) -> None:
     """
     Download and cache indexes from object storage for use with hostile clean
 
-    :arg filename: filename of index to download
+    :arg name: name of index to download
     :arg aligner: aligner(s) for which to download an index
     :arg list: list available indexes
     """
-    logging.info(f"Cache directory: {util.XDG_DATA_DIR}")
+    logging.info(f"Cache directory: {util.CACHE_DIR}")
     logging.info(f"Manifest URL: {util.BUCKET_URL}/manifest.json")
     if list:
         manifest = util.fetch_manifest()
         for name in manifest.keys():
             print(name)
     else:
         if aligner == "minimap2" or aligner == "both":
+            logging.info(f"Looking for Minimap2 index {name}")
             lib.ALIGNER.minimap2.value.check_index(name)
         if aligner == "bowtie2" or aligner == "both":
+            logging.info(f"Looking for Bowtie2 index {name}")
             lib.ALIGNER.bowtie2.value.check_index(name)
 
 
 def main():
     defopt.run(
         {"clean": clean, "mask": mask, "fetch": fetch},
         no_negated_flags=True,
```

### Comparing `hostile-1.0.0/src/hostile/lib.py` & `hostile-1.1.0/src/hostile/lib.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 @dataclass
 class SampleReport:
     version: str
     aligner: str
     index: str
-    options: str
+    options: list[str]
     fastq1_in_name: str
     fastq1_in_path: str
     fastq1_out_name: str
     fastq1_out_path: str
     reads_in: int
     reads_out: int
     reads_removed: int
@@ -41,15 +41,15 @@
 def gather_stats(
     rename: bool,
     reorder: bool,
     fastqs: list[Path],
     out_dir: Path,
     aligner: str,
     invert: bool,
-    index: Path | None,
+    index: str,
 ) -> list[dict[str, str | int | float | list[str]]]:
     stats = []
     for fastq1 in fastqs:
         fastq1_stem = util.fastq_path_to_stem(fastq1)
         fastq1_out_path = out_dir / f"{fastq1_stem}.clean.fastq.gz"
         n_reads_in_path = out_dir / (fastq1_stem + ".reads_in.txt")
         n_reads_out_path = out_dir / (fastq1_stem + ".reads_out.txt")
@@ -58,29 +58,23 @@
         n_reads_removed = n_reads_in - n_reads_out
         n_reads_in_path.unlink()
         n_reads_out_path.unlink()
         try:
             proportion_removed = round(n_reads_removed / n_reads_in, 5)
         except ArithmeticError:  # ZeroDivisionError
             proportion_removed = float(0)
-        index_fmt = (
-            index
-            if index
-            else Path(ALIGNER[aligner].value.data_dir)
-            / Path(ALIGNER[aligner].value.idx_name)
-        )
         options = [
             k
             for k, v in {"rename": rename, "reorder": reorder, "invert": invert}.items()
             if v
         ]
         report = SampleReport(
             version=__version__,
             aligner=aligner,
-            index=str(index_fmt),
+            index=index,
             options=options,
             fastq1_in_name=fastq1.name,
             fastq1_in_path=str(fastq1),
             fastq1_out_name=fastq1_out_path.name,
             fastq1_out_path=str(fastq1_out_path),
             reads_in=n_reads_in,
             reads_out=n_reads_out,
@@ -93,15 +87,15 @@
 
 def gather_stats_paired(
     rename: bool,
     reorder: bool,
     fastqs: list[tuple[Path, Path]],
     out_dir: Path,
     aligner: str,
-    index: Path | None,
+    index: str,
     invert: bool,
 ) -> list[dict[str, str | int | float]]:
     stats = []
     for fastq1, fastq2 in fastqs:
         fastq1_stem = util.fastq_path_to_stem(fastq1)
         fastq2_stem = util.fastq_path_to_stem(fastq2)
         fastq1_out_path = out_dir / f"{fastq1_stem}.clean_1.fastq.gz"
@@ -113,30 +107,24 @@
         n_reads_removed = n_reads_in - n_reads_out
         n_reads_in_path.unlink()
         n_reads_out_path.unlink()
         try:
             proportion_removed = round(n_reads_removed / n_reads_in, 5)
         except ArithmeticError:  # ZeroDivisionError
             proportion_removed = float(0)
-        index_fmt = (
-            index
-            if index
-            else Path(ALIGNER[aligner].value.data_dir)
-            / Path(ALIGNER[aligner].value.idx_name)
-        )
         options = [
             k
             for k, v in {"rename": rename, "reorder": reorder, "invert": invert}.items()
             if v
         ]
         stats.append(
             SampleReport(
                 version=__version__,
                 aligner=aligner,
-                index=str(index_fmt),
+                index=index,
                 options=options,
                 fastq1_in_name=fastq1.name,
                 fastq2_in_name=fastq2.name,
                 fastq1_in_path=str(fastq1),
                 fastq2_in_path=str(fastq2),
                 fastq1_out_name=fastq1_out_path.name,
                 fastq2_out_name=fastq2_out_path.name,
@@ -149,32 +137,30 @@
             ).__dict__
         )
     return stats
 
 
 def clean_fastqs(
     fastqs: list[Path],
-    index: str = "human-t2t-hla",
+    index: str = util.DEFAULT_INDEX_NAME,
     invert: bool = False,
     rename: bool = False,
     reorder: bool = False,
     out_dir: Path = util.CWD,
     aligner: ALIGNER = ALIGNER.minimap2,
     aligner_args: str = "",
     threads: int = util.THREADS,
     force: bool = False,
     offline: bool = False,
 ):
     logging.debug(f"clean_fastqs() {threads=}")
     if aligner == ALIGNER.bowtie2:
-        logging.info(f"Hostile version {__version__}. Using Bowtie2")
+        logging.info(f"Hostile version {__version__}. Mode: short read (Bowtie2)")
     elif aligner == ALIGNER.minimap2:
-        logging.info(
-            f"Hostile version {__version__}. Using Minimap2's long read preset"
-        )
+        logging.info(f"Hostile version {__version__}. Mode: long read (Minimap2)")
     fastqs = [Path(path).absolute() for path in fastqs]
     if not all(fastq.is_file() for fastq in fastqs):
         raise FileNotFoundError("One or more fastq files do not exist")
     Path(out_dir).mkdir(exist_ok=True, parents=True)
     index_path = aligner.value.check_index(index, offline=offline)
     backend_cmds = [
         aligner.value.gen_clean_cmd(
@@ -206,31 +192,33 @@
     util.fix_empty_fastqs(stats)
     logging.info("Cleaning complete")
     return stats
 
 
 def clean_paired_fastqs(
     fastqs: list[tuple[Path, Path]],
-    index: str = "human-t2t-hla",
+    index: str = util.DEFAULT_INDEX_NAME,
     invert: bool = False,
     rename: bool = False,
     reorder: bool = False,
     out_dir: Path = util.CWD,
     aligner: ALIGNER = ALIGNER.bowtie2,
     aligner_args: str = "",
     threads: int = util.THREADS,
     force: bool = False,
     offline: bool = False,
 ):
     logging.debug(f"clean_paired_fastqs() {threads=}")
     if aligner == ALIGNER.bowtie2:
-        logging.info(f"Hostile version {__version__}. Using Bowtie2 (paired reads)")
+        logging.info(
+            f"Hostile version {__version__}. Mode: paired short read (Bowtie2)"
+        )
     elif aligner == ALIGNER.minimap2:
         logging.info(
-            f"Hostile version {__version__}. Using Minimap2's short read preset (paired reads)"
+            f"Hostile version {__version__}. Mode: paired short read (Minimap2)"
         )
     fastqs = [
         (Path(path1).absolute(), Path(path2).absolute()) for path1, path2 in fastqs
     ]
     if not all(path.is_file() for fastq_pair in fastqs for path in fastq_pair):
         raise FileNotFoundError("One or more fastq files do not exist")
     Path(out_dir).mkdir(exist_ok=True, parents=True)
```

### Comparing `hostile-1.0.0/src/hostile/util.py` & `hostile-1.1.0/src/hostile/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import concurrent.futures
 import gzip
 import hashlib
 import logging
 import multiprocessing
+import os
 import platform
 import subprocess
 import tarfile
 
 import dnaio
 
 from pathlib import Path
@@ -16,58 +17,73 @@
 
 from tqdm import tqdm
 
 
 def choose_default_thread_count(cpu_count: int) -> int:
     """Choose a sensible number of threads for alignment"""
     cpu_count = int(cpu_count)
-    if cpu_count == 1:
+    if cpu_count <= 1:
         return 1
     elif 1 < cpu_count < 17:
         return int(cpu_count / 2)
-    elif cpu_count > 16:
+    else:
         return 10
 
 
 CWD = Path.cwd()
-XDG_DATA_DIR = Path(user_data_dir("hostile", "Bede Constantinides"))
+CACHE_DIR = (
+    Path(os.environ.get("HOSTILE_CACHE_DIR"))
+    if os.environ.get("HOSTILE_CACHE_DIR")
+    else Path(user_data_dir("hostile", "Bede Constantinides"))
+)
 CPU_COUNT = multiprocessing.cpu_count()
 THREADS = choose_default_thread_count(CPU_COUNT)
 BUCKET_URL = "https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o"
+DEFAULT_INDEX_NAME = "human-t2t-hla"
 
 
 def run(cmd: str, cwd: Path | None = None) -> subprocess.CompletedProcess:
     return subprocess.run(
         cmd, shell=True, cwd=cwd, check=True, text=True, capture_output=True
     )
 
 
 def run_bash(cmd: str, cwd: Path | None = None) -> subprocess.CompletedProcess:
     """Needed because /bin/sh does not support process substitution used for tee"""
+    cmd_fmt = f"set -o pipefail; {cmd}"
     return subprocess.run(
-        ["/bin/bash", "-c", cmd], cwd=cwd, check=True, text=True, capture_output=True
+        ["/bin/bash", "-c", cmd_fmt],
+        cwd=cwd,
+        check=True,
+        text=True,
+        capture_output=True,
     )
 
 
 def handle_alignment_exceptions(exception: subprocess.CalledProcessError) -> None:
     """Catch samtools view's non-zero exit if all input reads are contaminated"""
+    logging.debug(f"stdout: {exception.stdout}")
+    logging.debug(f"stderr: {exception.stderr}")
     alignment_successful = False
     stream_empty = False
     if 'Failed to read header for "-"' in exception.stderr:
         stream_empty = True
     if "overall alignment rate" in exception.stderr:  # Bowtie2
         alignment_successful = True
     if "Peak RSS" in exception.stderr:  # Minimap2
         alignment_successful = True
     if alignment_successful and stream_empty:  # Non zero exit but actually fine
         logging.debug("Alignment complete, empty SAM stream, continuing")
         pass
     else:
-        logging.error("Hostile encountered a problem. Stderr below")
-        print(f"{exception.stderr}")
+        logging.error(
+            f"Hostile encountered a problem. Check available RAM and storage\n"
+            f"pipeline stdout:\n{exception.stdout}\n"
+            f"pipeline stderr:\n{exception.stderr}\n"
+        )
         raise exception
 
 
 def run_bash_parallel(
     cmds: list[str], description: str = "Processing"
 ) -> dict[int, subprocess.CompletedProcess]:
     with concurrent.futures.ThreadPoolExecutor(max_workers=1) as x:
@@ -102,15 +118,15 @@
     except ValueError:  # file is empty and count is zero
         logging.debug(f"Count file missing: {path}")
         count = 0
     logging.debug(f"{path=} {count=}")
     return count
 
 
-def fetch_manifest(url: str = BUCKET_URL) -> list[str]:
+def fetch_manifest(url: str = BUCKET_URL) -> dict:
     logging.debug("Fetching bucket contents")
     try:
         r = httpx.get(f"{url}/manifest.json")
         r.raise_for_status()
     except httpx.HTTPError:
         raise httpx.HTTPError(
             "Failed to fetch manifest.json from object storage."
@@ -154,15 +170,15 @@
 
 
 def write_empty_gzip_text_file(path: Path) -> None:
     with gzip.open(path, "wt") as fh:
         fh.write("")
 
 
-def fix_empty_fastqs(stats) -> list[dict[str, str | int | float | list[str]]]:
+def fix_empty_fastqs(stats) -> None:
     """Find for empty output FASTQs and overwrite them with valid empty gzipped files"""
     for stat in stats:
         if stat.get("reads_out") == 0:
             fastq1_path = stat.get("fastq1_out_path")
             fastq2_path = stat.get("fastq2_out_path")
             if fastq1_path and Path(fastq1_path).is_file():
                 write_empty_gzip_text_file(fastq1_path)
```

### Comparing `hostile-1.0.0/tests/data/mask/gallid-herpesvirus-2.fa` & `hostile-1.1.0/tests/data/mask/gallid-herpesvirus-2.fa`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/mask/t2t-chm13v2.0-chr21-subset.fa` & `hostile-1.1.0/tests/data/mask/t2t-chm13v2.0-chr21-subset.fa`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/partial-for-mask-testing.fa.gz` & `hostile-1.1.0/tests/data/sars-cov-2/partial-for-mask-testing.fa.gz`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.1.bt2` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.2.bt2` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.4.bt2` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.4.bt2`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.fasta.gz` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.fasta.gz`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.rev.1.bt2` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.rev.1.bt2`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2/sars-cov-2.rev.2.bt2` & `hostile-1.1.0/tests/data/sars-cov-2/sars-cov-2.rev.2.bt2`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2_100_1.fastq.gz` & `hostile-1.1.0/tests/data/sars-cov-2_100_1.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2_100_2.fastq.gz` & `hostile-1.1.0/tests/data/sars-cov-2_100_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/sars-cov-2_50_2.fastq.gz` & `hostile-1.1.0/tests/data/sars-cov-2_50_2.fastq.gz`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/data/tuberculosis_2.fastq` & `hostile-1.1.0/tests/data/tuberculosis_2.fastq`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/tests/test_all.py` & `hostile-1.1.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `hostile-1.0.0/PKG-INFO` & `hostile-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hostile
-Version: 1.0.0
+Version: 1.1.0
 Summary: Accurate host read removal
 Author-email: Bede Constantinides <b@bede.im>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: defopt>=6.4.0
 Requires-Dist: dnaio>=1.2.0
@@ -21,28 +21,28 @@
 
 <p align="center">
     <img width="250" src="logo.png">
 </p>
 
 # Hostile
 
-Hostile accurately removes host sequences from short and long read (meta)genomes, consuming paired or unpaired `fastq[.gz]` input. Batteries are included – a human reference genome is downloaded when run for the first time. Hostile is precise by default, removing an [order of magnitude fewer microbial reads](https://log.bede.im/2023/08/29/precise-host-read-removal.html#evaluating-accuracy) than existing approaches while removing >99.5% of real human reads from 1000 Genomes Project samples. For the best possible retention of microbial reads, use an existing index masked against bacterial and/or viral genomes, or make your own using the built-in masking utility. Read headers can be replaced with integers (using `--rename`) for privacy and smaller FASTQs. Heavy lifting is done with fast existing tools (Minimap2/Bowtie2 and Samtools). Bowtie2 is the default aligner for short (paired) reads while Minimap2 is default aligner for long reads. In benchmarks, bacterial Illumina reads were decontaminated at 32Mbp/s (210k reads/sec) and bacterial ONT reads at 22Mbp/s, using 8 alignment threads. Further information and benchmarks can be found in the [paper](https://doi.org/10.1093/bioinformatics/btad728) and [blog post](https://log.bede.im/2023/08/29/precise-host-read-removal.html). Please open an issue to report problems [or](mailto:b@bede.im) [otherwise](https://twitter.com/beconsta) [reach](https://bsky.app/profile/bedec.bsky.social) [out](https://mstdn.science/@bede) for help, advice etc.
+Hostile accurately removes host sequences from short and long read (meta)genomes, consuming paired or unpaired `fastq[.gz]` input. Batteries are included – a human reference genome is downloaded when run for the first time. Hostile is precise by default, removing an [order of magnitude fewer microbial reads](https://log.bede.im/2023/08/29/precise-host-read-removal.html#evaluating-accuracy) than existing approaches while removing >99.5% of real human reads from 1000 Genomes Project samples. For the best possible retention of microbial reads, use an existing index masked against bacterial and/or viral genomes, or make your own using the built-in masking utility. Read headers can be replaced with integers (using `--rename`) for privacy and smaller FASTQs. Heavy lifting is done with fast existing tools (Minimap2/Bowtie2 and Samtools). Bowtie2 is the default aligner for short (paired) reads while Minimap2 is default aligner for long reads. In benchmarks, bacterial Illumina reads were decontaminated at 32Mbp/s (210k reads/sec) and bacterial ONT reads at 22Mbp/s, using 8 alignment threads. By default, Hostile requires 4GB of RAM for decontaminating short reads and 13GB for long reads (Minimap2). Further information and benchmarks can be found in the [paper](https://doi.org/10.1093/bioinformatics/btad728) and [blog post](https://log.bede.im/2023/08/29/precise-host-read-removal.html). Please open an issue to report problems [or](mailto:b@bede.im) [otherwise](https://twitter.com/beconsta) [reach](https://bsky.app/profile/bedec.bsky.social) [out](https://mstdn.science/@bede) for help, advice etc.
 
 
 
 ## Reference genomes (indexes)
 
-The default index `human-t2t-hla` comprises [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) and [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51, and is downloaded automatically when running Hostile unless another index is specified. Slightly higher microbial sequence retention is possible using a masked index, of which several are available. The index `human-t2t-hla-argos985` is masked against [985 reference grade bacterial genomes](https://www.ncbi.nlm.nih.gov/bioproject/231221) including common human pathogens, while `human-t2t-hla-argos985-mycob140` is further masked against mycobacterial genomes. To use a standard index, simply pass its name as the value of the `--index` argument which takes care of downloading and cacheing the relevant index. Automatic download can be disabled using the `--offline` flag, and `--index` can accept a path to a custom reference genome or Bowtie2 index. [Object storage](https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o) is provided by the [ModMedMicro research group](https://www.expmedndm.ox.ac.uk/modernising-medical-microbiology).
+The default index `human-t2t-hla` comprises [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) and [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51, and is downloaded automatically when running Hostile unless another index is specified. Slightly higher microbial sequence retention is may be possible using masked indexes, listed below. The index `human-t2t-hla-argos985` is masked against [985 reference grade bacterial genomes](https://www.ncbi.nlm.nih.gov/bioproject/231221) including common human pathogens, while `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` is further masked comoprehensively against all known virus and phage genomes. The latter should be used when retention of viral sequences is a priority. To use a standard index, simply pass its name as the value of the `--index` argument which takes care of downloading and caching the relevant index. Automatic download can be disabled using the `--offline` flag, and `--index` can accept a path to a custom reference genome or Bowtie2 index. [Object storage](https://objectstorage.uk-london-1.oraclecloud.com/n/lrbvkel2wjot/b/human-genome-bucket/o) is provided by the [ModMedMicro research unit](https://www.expmedndm.ox.ac.uk/modernising-medical-microbiology) at the University of Oxford.
 
 |                             Name                             |                         Composition                          | Date    | Masked positions       |
 | :----------------------------------------------------------: | :----------------------------------------------------------: | ------- | ---------------------- |
 |                `human-t2t-hla` **(default)**                 | [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/11828891) + [IPD-IMGT/HLA](https://www.ebi.ac.uk/ipd/imgt/hla/) v3.51 | 2023-07 | 0 (**0%**)             |
 |                   `human-t2t-hla-argos985`                   | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial** genomes | 2023-07 | 317,973 (**0.010%**)   |
 |       `human-t2t-hla.rs-viral-202401_ml-phage-202401`        | `human-t2t-hla` masked with 150mers for 18,719 RefSeq **viral** and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,172,993 (**0.037%**) |
-| `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) bacterial, 18,719 RefSeq **viral**, and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,473,260 (**0.046%**) |
+| `human-t2t-hla.argos-bacteria-985_rs-viral-202401_ml-phage-202401` | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial**, 18,719 RefSeq **viral**, and 26,928 [Millard Lab **phage**](https://millardlab.org/phage-genomes-jan-2024/) genomes | 2024-01 | 1,473,260 (**0.046%**) |
 |              `human-t2t-hla-argos985-mycob140`               | `human-t2t-hla` masked with 150mers for [985](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) [FDA-ARGOS](https://www.ncbi.nlm.nih.gov/bioproject/231221) **bacterial** & [140](https://github.com/bede/hostile/blob/main/paper/supplementary-table-2.tsv) **mycobacterial** genomes | 2023-07 | 319,752 (**0.010%**)   |
 
 *Performance of `human-t2t-hla` and `human-t2t-hla-argos985-mycob140` was evaluated in the [paper](https://doi.org/10.1093/bioinformatics/btad728)*
 
 
 
 ## Install  [![Install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat-square&logo=anaconda)](https://biocontainers.pro/tools/hostile) [![Install with Docker](https://img.shields.io/badge/install%20with-docker-important.svg?style=flat-square&logo=docker)](https://biocontainers.pro/tools/hostile)
@@ -55,52 +55,53 @@
 conda create -y -n hostile -c conda-forge -c bioconda hostile
 conda activate hostile
 ```
 
 **Docker**
 
 ```bash
-docker run quay.io/biocontainers/hostile:0.4.0--pyhdfd78af_0
-
-# Build your own
 wget https://raw.githubusercontent.com/bede/hostile/main/Dockerfile
 docker build . --platform linux/amd64
 ```
 
+A [Biocontainer image](https://biocontainers.pro/tools/hostile) is also available, but beware that this often lags behind the latest released version
+
 
 
 ## Index installation (optional)
 
 Hostile automatically downloads and caches the default index `human-t2t-hla` when run for the first time, meaning that there is no need to download an index in advance. Neverthless:
 
 - To download and cache the default index (`human-t2t-hla`), run `hostile fetch`
 - To list available indexes, run `hostile fetch --list`
 - To download and cache another standard index, run e.g. `hostile fetch --name human-t2t-hla-argos985`
-- To use a custom genome (made perhaps with `hostile mask`), run `hostile clean --index path/to/genome.fa`
+- To use a custom genome (made with e.g. `hostile mask`), run `hostile clean` with  `--index path/to/genome.fa` (minimap2) or `--index path/to/index` (without file extensions; Bowtie2)
+- To change where indexes are stored, set the environment variable `HOSTILE_CACHE_DIR` to a directory of your choice. Run `hostile fetch --list` to verify.
 
 
 
 ## Command line usage
 
 ```bash
 $ hostile clean -h
-usage: hostile clean [-h] --fastq1 FASTQ1 [--fastq2 FASTQ2] [--aligner {bowtie2,minimap2,auto}] [--index INDEX] [--invert] [--rename] [--reorder] [--out-dir OUT_DIR] [--threads THREADS] [--aligner-args ALIGNER_ARGS] [--force]
-                     [--offline] [--debug]
+usage: hostile clean [-h] --fastq1 FASTQ1 [--fastq2 FASTQ2] [--aligner {bowtie2,minimap2,auto}] [--index INDEX]
+                     [--invert] [--rename] [--reorder] [--out-dir OUT_DIR] [--threads THREADS]
+                     [--aligner-args ALIGNER_ARGS] [--force] [--offline] [--debug]
 
-Remove reads aligning to a target genome from fastq[.gz] input files.
+Remove reads aligning to an index from fastq[.gz] input files
 
 options:
   -h, --help            show this help message and exit
   --fastq1 FASTQ1       path to forward fastq[.gz] file
   --fastq2 FASTQ2       optional path to reverse fastq[.gz] file
                         (default: None)
   --aligner {bowtie2,minimap2,auto}
                         alignment algorithm. Default is Bowtie2 (paired reads) & Minimap2 (unpaired reads)
                         (default: auto)
-  --index INDEX         name of standard index or path to custom index
+  --index INDEX         name of standard index or path to custom genome/index
                         (default: human-t2t-hla)
   --invert              keep only reads aligning to the target genome (and their mates if applicable)
                         (default: False)
   --rename              replace read names with incrementing integers
                         (default: False)
   --reorder             ensure deterministic output order
                         (default: False)
@@ -121,16 +122,16 @@
 
 
 
 **Short reads, default index**
 
 ```bash
 $ hostile clean --fastq1 human_1_1.fastq.gz --fastq2 human_1_2.fastq.gz
-INFO: Hostile version 1.0.0. Using Bowtie2 (paired reads)
-INFO: Found cached standard index human-t2t-hla (Bowtie2)
+INFO: Hostile version 1.0.0. Mode: paired short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 [
     {
         "version": "1.0.0",
         "aligner": "bowtie2",
         "index": "human-t2t-hla",
@@ -146,32 +147,48 @@
         "fastq2_in_name": "human_1_2.fastq.gz",
         "fastq2_in_path": "/Users/bede/human_1_2.fastq.gz",
         "fastq2_out_name": "human_1_2.clean_2.fastq.gz",
         "fastq2_out_path": "/Users/bede/human_1_2.clean_2.fastq.gz"
     }
 ]
 ```
+
+
 **Short reads, masked index, save log**
 
 ```bash
 $ hostile clean --fastq1 human_1_1.fastq.gz --fastq2 human_1_2.fastq.gz --index human-t2t-hla-argos985 > log.json
-INFO: Hostile version 1.0.0. Using Bowtie2 (paired reads)
-INFO: Found cached standard index human-t2t-hla (Bowtie2)
+INFO: Hostile version 1.0.0. Mode: paired short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
+INFO: Cleaning…
+INFO: Cleaning complete
+```
+
+
+
+**Short unpaired reads, save log**
+
+By default, single fastqs are assumed to be long reads. Override this by specifying `--aligner bowtie2` when decontaminating unpaired short reads.
+
+```bash
+$ hostile clean --aligner bowtie2 --fastq1 tests/data/human_1_1.fastq.gz > log.json
+INFO: Hostile version 1.0.0. Mode: short read (Bowtie2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 ```
 
 
 
 **Long reads**
 
 ```bash
 $ hostile clean --fastq1 tests/data/tuberculosis_1_1.fastq.gz
-INFO: Hostile version 1.0.0. Using Minimap2's long read preset
-INFO: Found cached standard index human-t2t-hla (Minimap2)
+INFO: Hostile version 1.0.0. Mode: long read (Minimap2)
+INFO: Found cached standard index human-t2t-hla
 INFO: Cleaning…
 INFO: Cleaning complete
 [
     {
         "version": "1.0.0",
         "aligner": "minimap2",
         "index": "human-t2t-hla",
@@ -223,17 +240,18 @@
 ```bash
 hostile mask human.fasta lots-of-bacterial-genomes.fasta --threads 8
 ```
 You may wish to use one of the existing [reference genomes](#reference-genomes--indexes) as a starting point. Masking uses Minimap2 to align 150mers of the supplied target genomes with the reference genome, and bedtools to mask all aligned regions with N. Both a masked genome (for Minimap2) and a masked Bowtie2 index is created.
 
 
 
-## Known issues
+## Limitations
 
-- Using more than 10 alignment threads may reduce performance, even on systems with enough CPU cores. A sensible default is therefore chosen automatically at runtime. To maximise performance on your system, some experimentation may be necessary.
+- Hostile prioritises retaining microbial sequences above discarding host sequences. If you strive to remove every last human sequence, other approaches may serve you better.
+- Performance is not always improved by using all available CPU cores. A sensible default is therefore chosen automatically at runtime based on the number of available CPU cores.
 - Minimap2 has an overhead of 30-90s for human genome indexing prior to starting decontamination. Surprisingly, loading a prebuilt index is not significantly faster. I hope to mitigate this in a future release.
 
 
 
 ## Citation
 
 Bede Constantinides, Martin Hunt, Derrick W Crook,  Hostile: accurate decontamination of microbial host sequences, *Bioinformatics*, 2023; btad728, https://doi.org/10.1093/bioinformatics/btad728
```

