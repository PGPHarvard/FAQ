# Navigation

* [Back to FAQ Home](README.md)
* [Back to Harvard PGP Home](http://my.pgp-hms.org)

# Researcher FAQ

### Data Access for Harvard PGP Data

The Harvard Personal Genome Project participant page, located at [my.pgp-hms.org](https://my.pgp-hms.org), holds information on participant data.
Each Harvard Personal Genome Project participant has a profile page listing their available information.
For example, the [profile participant for hu43860C](https://my.pgp-hms.org/profile/hu43860C) has medical information,
the results of surveys provided by the Harvard Personal Genome Project and links to data files associated with this
participant, including whole genome data and genotype data.

The Harvard Personal Genome Project can be used to search for:

* [participant profiles](https://my.pgp-hms.org/users)
* [participant surveys](https://my.pgp-hms.org/google_surveys)
* [specimens](https://my.pgp-hms.org/specimens)
* [public genetic data](https://my.pgp-hms.org/public_genetic_data)

among others.  Please consult the [Harvard Personal Genome Project page](https://my.pgp-hms.org/) for more detail.

In addition to the Harvard Personal Genome Project site, there is a consolidated database of the Harvard PGP available for download:

* [Consolidated Database for the Harvard PGP](https://workbench.su92l.arvadosapi.com/collections/3ccedff14c04af4d96e41e96648c55e2+3173/html/index.html)

Available in the above link is a SQLite3 database (around 140Mb uncompressed) that holds information available from participant profiles along with data retrieved from participant GET-Evidence reports.  Also available are the comma and tab space delimited files used to create the SQLite3 database.  Data is periodically retrieved from the Harvard PGP site and the above link represents the most recent snapshot of the database taken.

The spreadsheets and SQLite3 database only represent most of the data provided by the participants profile, including phenotype data, health record information and genome file locations.  URLs to full genomic data and participant uploaded data (such as 23andMe genotype data, etc.) can be found from participants profiles as well as consulting the appropriate entries in the above consolidated database.  For an introduction to the above database and visualization tool, see the [untap Introduction page](https://github.com/abeconnelly/untap/blob/master/Introduction.md).

Source code for download and presentation of the above database can be found on the [untap](https://github.com/abeconnelly/untap) repository.

### Where can I get the FASTQ/BAM/VCF/etc. files?

Most genomic data available through the Harvard Personal Genome Project site is only available in the format provided to us by Complete Genomics (CGI) and would need to be converted.

CGI gives us unaligned read information, variant evidence files and CGI-Var files, among others.
All other file formats (e.g. SAM, BAM, FASTQ, VCF, etc.) are not directly provided for released whole genome data and would need to be derived by using other tools.

CGI provides a suite of tools for use in analyzing and converting their data called [cgatools](http://cgatools.sourceforge.net/).
Some of the data files provided to us by CGI are not available through participant profiles but are available through an [Arvados collection](https://workbench.su92l.arvadosapi.com/projects/su92l-j7d0g-nf54gdds5jj03tc#Data_collections) and mirrored on a [Google drive](https://console.developers.google.com/storage/browser/pgp-harvard-data-public/).
For information on accessing data on the Google drive, please see [a blog post we've written](http://blog.personalgenomes.org/2014/05/30/pgp-harvard-data-in-google-cloud-storage/) about it.
In the future this may change, but due to space concerns, we do not make available the unaligned read information provided to us by CGI.

Participants are allowed to upload any data they like, which includes FASTQ and BAM files, among others.
This means that some data in other formats, such as BAM or FASTQ, is available because a participant uploaded the
data themselves.
Feel free to search the Harvard Personal Genome Project site for any additional genomic data that you might find useful.
For example, looking for FASTQ on the [public genetic data page](https://my.pgp-hms.org/public_genetic_data) shows a few participant uploaded FASTQ files.
### Who should I contact if run into problems/need help/have other questions

Please feel free to contact us by [filling out a contact form](http://personalgenomes.org/harvard/contact-us) on the [PersonalGenomes.org](http://personalgenomes.org/harvardh) website.
