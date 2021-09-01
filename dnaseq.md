## DNA Sequencing

(TODO: complete notes, restructure)


 1. Machine creates [Base Call File (BCL)](https://support.illumina.com/bulletins/2016/04/fastq-files-explained.html).
 2. Machine developer transforms BCL to [FASTQ (.fq, .fastq)](https://support.illumina.com/bulletins/2016/04/fastq-files-explained.html). I.e., customer gets fastq files, often gzipped as they are huge (.fastq.gz).
 3. Reference genomes are provided with [FASTA (.fa)](https://en.wikipedia.org/wiki/FASTA_format) files. Examples are [hg19](https://www.ncbi.nlm.nih.gov/assembly/GCF_000001405.13/) and [hg38](https://www.ncbi.nlm.nih.gov/assembly/GCF_000001405.26/).
 4. [Sequence Alignment Map (SAM/BAM/SCRAM)](https://en.wikipedia.org/wiki/SAM_(file_format)) > [Variant Call Format (VCF)](https://en.wikipedia.org/wiki/Variant_Call_Format) > [Binary 


[Differences between FASTA FASTQ and SAM](https://bioinformatics.stackexchange.com/questions/14/what-is-the-difference-between-fasta-fastq-and-sam-file-formats?newreg=5d7230bde2c64766838c3086157b4342)

 * FASTA: sequence records
 * FASTQ: FASTA+Quality info
 * SAM: FASTQ + mapping info (as TSV)
 * BAM: SAM as binary + search index

[BAM compressed with GZIP (.bgzf)](https://biopython.org/docs/1.75/api/Bio.bgzf.html)

[Tabix (.tbi)](http://www.htslib.org/doc/tabix.html) for indexing and then fast retrieval of slices from big files.


[VCF and BCF (TODO)](https://samtools.github.io/bcftools/howtos/variant-calling.html)



called
cleaned (filtered for quality, etc)
ancestral/derived snips
