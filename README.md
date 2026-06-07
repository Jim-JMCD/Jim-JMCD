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
_________________________________________________________________________________________________________________________
#### [genFRN](https://github.com/Jim-JMCD/genFRN) - _Generic File Re-namer_
  
A script ( Bash & Powershell) that renames files, in a directory, that have generic meaningless names produced by phones, cameras log file genrators. This script will add the names of the parent directories as a prefix to current names. The script creates an executable log that will undo the renaming processing. The number of parent directory names you want to include in the prefix of the new name is selectable. 
_________________________________________________________________________________________________________________________
#### [mutt_protonmail-bridge](https://github.com/Jim-JMCD/mutt_protonmail-bridge) _for Linux Server & Desktop_
##### Guide for installing, configuring and using the Mutt mail client with Proton Mail Bridge on Linux Server and Linux Desktop.

System, security and application administrators use command line mail tools like sendmail, postfix, mailx and mutt to mail out reports alerts and other material to people that presumably care. This guide describes how setup up command line mail services using Proton Mail Bridge combined with the Mutt mail client. Mutt is an option for those that do not have a personal domian.

[Mutt_Proton_Mail-Bridge_Guide (PDF)](https://github.com/Jim-JMCD/mutt_protonmail-bridge/blob/main/Mutt_Proton_Mail-Bridge_Guide.pdf) The repo contins the muttrc and scripts
_________________________________________________________________________________________________________________________
#### [Data Dedupe calculator](https://github.com/Jim-JMCD/Data_storage_network_deduplication_calculator) _for Storage & Network capacity planning and requirements_
Calculations are theoretical and used to illustrate the dynamics of the impact deduplication.  Calcultor out will not likely to match vendor calculations because there are many factors that influence deduplication capacity planning.

Download [Data dedupe calculator (MS-Excel)](https://github.com/Jim-JMCD/Data_storage_network_deduplication_calculator/blob/main/Dedupecal_202308L.xlsx) macro free. The repro has examples of usage.
_________________________________________________________________________________________________________________________


