## downsizeVCF

A quick script to take a vcf file and return a downsized version of that file. Useful for testing purposes before running new pipelines on larger vcf files.

Located at /re_gecip/neurology/THRK/downsizeVCF

The script takes any vcf file (compressed or not) and uses bcftools to copy across all header information, then takes every 100th variant row, up to a maximum of 200 variants.

In GeL, run with:

	bsub < downsize_vcf.sh