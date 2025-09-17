# workflow-commands.md 
# 1 Download SRA Toolkit 
To install SRA toolkit use command `sudo apt-get install sra-toolkit`
To check download use command `vdb-dump -version`
# 2 To download SRA FILE Raw reads 
use command `prefetch SRR23515036`
# 3 convert SRA file into FASTQ 
use command `fastq-dump SRR23515036` For paired end data
# 4 To split file
use `fastq-dump --split-files SRR23515036` 
to check fastq file use `head SRR23515036`
# 5 To download FASTQC program 
use command `sudo apt install fastqc`
to change directory `cd fastqc`
to give permission use `chmod+rwxfastqc`
to run the file use `./`
# 6 To install Fastp
use command `apt install fastp`
To give permission `chmod+x fastp`
to make script `nano fastp.sh`
To write script use shebang `#!/usr/bin/bash`
Write path after shebang to write the script `/usr/bin/fastp fastp -i SRR23515036_1.fastq -o SRR23515036_1clean_fastq I - SRR23515036_2_fastq O SRR23515036 _2_Clean.fastq`
to run script use `./fastp.sh`
to view use `cat fastp.sh`
# 7 install Jellyfish tool for k-mer count 
use command `sudo apt install jellyfish`
to check install use `jellyfish -version`
use script

