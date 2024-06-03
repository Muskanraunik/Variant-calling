# Variant-calling
* variant calling is performed on WGS data
* It integrate various tools for quality control, alignment, BAM file manipulation, and gene expression quantification.
# Features
* Quality Control: Uses FastQC for initial quality assessment.
* Read Alignment: Employs Bowtie2 for aligning RNA-seq reads to a reference genome.
* BAM File Manipulation: Uses Samtools for sorting, indexing, and manipulating BAM files
# Adding Read Group
* picard.jar is used to annotate each read of sorted bam file with metadata describing the experimental conditions under which the read was generated. 
* It includes details such as the sequencing platform, library preparation protocol, sample identifier
* Read Group ID (RGID): A unique identifier for the read group.
* Read Group Library (RGLB): The library from which the sequencing data was generated.
* Read Group Platform (RGPL): The platform or technology used for sequencing.
* Read Group Platform Unit (RGPU): The platform unit, which typically includes information about the flowcell, barcode, and lane used for sequencing.
* Read Group Sample Name (RGSM): The name of the biological sample from which the sequencing data was generated.
# Variant calling
*  Calling variants  using GATKHaplotypeCaller
# Filteration
* Filteration is performed using GATK VariantFiltration.
# Annotation
* annovar.pl is used for annotating vcf file.
