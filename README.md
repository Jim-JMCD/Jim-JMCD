# Contents

#### [syncBKUP](https://github.com/Jim-JMCD/syncBKUP) - _Synchronised data backups with unlimited delta versioning_

_syncBKUP_, a Bash script to that synchronises data directories and files to a backup repository. Only the most recent backup is stored in the repository. All changes and deletion to any directory or file between backups are kept in individual version directories. There are no limits on how long or how much historical data is kept, its user managed.  This script is based on the capabilities of ***rsync***.
_________________________________________________________________________________________________________________________
#### [duplicateFF](https://github.com/Jim-JMCD/duplicateFF) - _Duplicate File Finder_
Duplicate file finder, a small Linux app (x86 & ARM) that produces reports on duplicate & unique files using sha256 checksum. Input can be one or more directories with optional filters of maximum files size and parts of file names. Output is multiple CSV (spreadsheet) reports that can be used to move or delete duplicates in Linux, Windows-WSL, MSYS2, Gitbash
_________________________________________________________________________________________________________________________
#### [testFilesCreate](https://github.com/Jim-JMCD/testFilesCreate) 
##### Create bulk data for testing and benchmarking data storage, backups, data compression and deduplication  
 A small Linux app that creates test files filling them with random data in a single directory or a directory tree. 
 * Includes a calculator for creating data in directory trees.
 * Can create a single file to a directory tree, tree size provided by user.  
 * File contents can either be printable or binary. All contents generated from /dev/urandom.
 * Selecting the printable pool of characters determines the **compressibility** of file contents.  
 * Files sizes can be identical or randomly sized within a given range.
 * Files can be identical or individually filled with random content.
 * Run either interactively or unaccompanied in batch mode.

 ___[TestFilesCreate Datasheet](https://github.com/Jim-JMCD/testFilesCreate/blob/main/Datasheet%20testFilesCreate.pdf)___ Usage plus results testing data compression and data deduplication 
__________________________________________________________________________________________________________________________
#### [tetsFilesMake](https://github.com/Jim-JMCD/testFilesMake)  

Similar to __testFilesCreate__. Differences being: only produces a single directory of test files, has an option for sparse files and no calculator.

Makes test data for testing data storage, compression and transfer. The app can create test data files filled random selectable printable characters or binary data. Selecting printable content controls how compressible the test data is. There is a sparse file option. Files are created in a single directory. No data creation limits. 
_________________________________________________________________________________________________________________________
#### [genFRN](https://github.com/Jim-JMCD/genFRN) - _Generic File Re-namer_
  
A script ( Bash & Powershell) that renames files, in a directory, that have generic meaningless names produced by phones, cameras log file genrators. This script will add the names of the parent directories as a prefix to current names. The script creates an executable log that will undo the renaming processing. The number of parent directory names you want to include in the prefix of the new name is selectable. 
_________________________________________________________________________________________________________________________
#### [Data Dedupe calculator](https://github.com/Jim-JMCD/Data_storage_network_deduplication_calculator) _for Storage & Network capacity planning and requirements_
Calculations are theoretical and used to illustrate the dynamics of the impact deduplication.  Calcultor out will not likely to match vendor calculations because there are many factors that influence deduplication capacity planning.

Download [Data dedupe calculator (MS-Excel)](https://github.com/Jim-JMCD/Data_storage_network_deduplication_calculator/blob/main/Dedupecal_202308L.xlsx) macro free. The repro has examples of usage.
________________________________________________________________________________________________________________________
# Guides for Linux Server and Desktop Mail Tools
System, security and application administrators use command line mail tools like sendmail, postfix, mailx and mutt to mail out reports, alerts and other material to external people. These guides describe how setup up command line mail services using Proton Mail Bridge and mail-only SMTP services.  SMTP services can used with Linux system utilities that are mail enabled, like cron.
________________________________________________________________________________________________________________________
## [Mutt with Proton Mail Bridge](https://github.com/Jim-JMCD/mutt_protonmail-bridge)
Guide for installing, configuring and using the Mutt mail client with Proton Mail Bridge.  Mutt is an option for those that do not have a domian to use.

[Mutt_Proton_Mail-Bridge_Guide (PDF)](https://github.com/Jim-JMCD/mutt_protonmail-bridge/blob/main/Mutt_Proton_Mail-Bridge_Guide.pdf) The repo contains the muttrc and scripts
_________________________________________________________________________________________________________________________
## [A Guide for integrating Postfix with Proton Mail & Scaleway TEM SMTP servcies.](https://github.com/Jim-JMCD/Postfix-SMTP_Guide_for_PROTONmail_and_SCALEWAY-TEM/blob/main/POSTFIX-SMTP_Guide_for_PROTONmail_and_SCALEWAY-TEM.pdf)
#### Proton STMP is an integrated mail relay add-on to a regular mail account, best for low volume mailing.
#### Scaleway transactional SMTP mail service is designed for low and high volume mailing.         

This guide describes how integrate Linux postfix to work with Proton Mail and Scaleway Transactional Email (TEM) secure SMTP services. Postfix when configured to work with a SMTP relay provides system and application administrators to use native and application mail tools to send reports, alerts and other information to external email addresses. The SMTP services of Proton and Scaleway are different in configuration requirements because they are designed for different workloads.    

The guide is for separate installations, it does not cover configuring postfix to use Proton and Scaleway SMTP in the same computer.   
 
##### Guide coverage
* Postfix Installation and configuration with SASL/TLS security.
* Setting default email addresses with __*sender_canonical*__. 
* Enabling preconfigured sender email addresses for Proton SMTP with __*sender_relay*__.
* Configuring cron and rsyslog ommail to send external mail.
* Testing and some troubleshooting.

This guide could be used for other Postfix SMTP mail installations. 

[A Guide for integrating Postfix with Proton Mail & Scaleway TEM SMTP servcies](https://github.com/Jim-JMCD/Postfix-SMTP_Guide_for_PROTONmail_and_SCALEWAY-TEM) The repo contians configuration files   
________________________________________________________________________________________________________________________

