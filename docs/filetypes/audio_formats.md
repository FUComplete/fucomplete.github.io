---
layout: default
title: Audio
parent: Formats
grand_parent: Documentation
nav_order: 2
---

# Audio
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

- TOC
{:toc}

## BD
File that stores appended headerless PSX (VAG) audio files.

Can decode using vgmstream and a txth to state the audio file settings. 

Create a file called ```.TXTH``` with the following in it:
```
codec = PSX
sample_rate = 16000
channels = 1
num_samples = data_size
```

## PHD

PHD files are effectively the header files for BD's and have 4 sections... ```Head```, ```Prog```, ```Smpl``` and ```Vagi```.

### Head

```cpp
struct HEADHeader{
    uint    FileID;
    uint    SizeOfHead;
    uint    Unk;
    uint    SizeOfPHD;
    uint    SizeOfBD;
    uint    ProgPTR
    uint    SmplPTR
    uint    VagiPTR
}
```

{: .note }
Could be that `Unk` is saying theres 3 sections after `Head`... that being `Prog`, `Smpl`, and `Vagi`.

### Vagi

```cpp
struct VAGIHeader{
    uint    FileID;
    uint    SizeOfVagi;
    uint    NumOfFiles;
    uint    TERM;
}
```

{: .note }
`TERM` seems to just terminate with `FF FF FF FF`

Followed by each file reference.

```cpp
struct VAGIFileRef{
    uint    Offset;
    uint    Size;
    uint    NULL;
    uint    Frequency;
    uint    NULL;
}
```

## AT3

Sony's generic ATRAC3 audio files

## CAF (iOS)

Generic Apple Core Audio Format used on iOS. 

