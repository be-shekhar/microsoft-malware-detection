# Microsoft Malware Detection

### Source: https://www.kaggle.com/c/malware-classification/

## Business Problem
In the past few years, the malware industry has grown very rapidly, this indicates that malwares nowadays evade traditional protection, forcing the anti-malware groups/communities to build more robust softwares to detect and terminate these attacks. The major part of protecting a computer system from a malware attack is to identify whether a given piece of file/software is a malware.

Microsoft has been very active in building anti-malware products over the years and it runs it’s anti-malware utilities over 150 million computers around the world. This generates tens of millions of daily data points to be analyzed as potential malware. In order to be effective in analyzing and classifying such large amounts of data, we need to be able to group them into groups and identify their respective families. 

## Problem Statement
The dataset provided by Microsoft contains about 9 classes of malware. The problem statement is to build a robust multi class classification model that can accurately classify which class a malware belongs to.

## Business Objectives and Constraints
1. Minimize multi-class error.
2. Multi-class probability estimates.
3. Malware detection should not take hours and block the user's computer. It should fininsh in a few seconds or a minute.

## Data Overview
1. For every malware, we have two files
    - .asm file (read more: https://www.reviversoft.com/file-extensions/asm)
    - .bytes file (the raw data contains the hexadecimal representation of the file's binary content, without the PE header)
2. Total train dataset consist of 200GB data out of which 50Gb of data is .bytes files and 150GB of data is .asm files:
3. Lots of Data for a single-box/computer.
4. There are total 10,868 .bytes files and 10,868 asm files total 21,736 files
5. There are 9 types of malwares (9 classes) in our give data
6. Types of Malware:
    - Ramnit
    - Lollipop
    - Kelihos_ver3
    - Vundo
    - Simda
    - Tracur
    - Kelihos_ver1
    - Obfuscator.ACY
    - Gatak
