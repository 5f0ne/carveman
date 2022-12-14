# Description

File carving for pictures, documents and other files based on it's header an footer signatures. Does work for non fragmented files only at the moment.

# Available Files:

- .jpg
- .png
- .pdf

# Installation

`pip install carveman`

# Usage

**From command line:**

`python -m carveman --path PATH [--outdir OUTDIR]`

| Option | Short | Type | Default | Description |
|---|---|---|---|---|
|--path | -p | String | - | Path to carving source (dd, raw) |
|--outdir | -o | String | carveman-result | Path to dir where carved files are located |


# Example

`python -m carveman -p path/to/carving-source/example.dd`

The carved files will be located in `carveman-result`

```

###########################################################################################

Carveman by 5f0
File carving for pictures, documents and other files based on it's file signatures

Current working directory: path/to/carveman
        Investigated file: example.dd

                      MD5: 9ff0c5b220e4345133181e7101571374
                   SHA256: b4864ce518b51e0fe6ee43cf705a5a39bedc97c25c97e857314b22b7d5e500a7

     Path to carved files: carveman-result

 Datetime: 01/01/1970 10:11:12

###########################################################################################

--> Carving started

--> Carving for: .jpg

------> .jpg detected! - Start Hex: 0x7000 - End Hex: 0xc1b0 - Nr: 1
------> .jpg detected! - Start Hex: 0xf000 - End Hex: 0x22d77 - Nr: 2
------> .jpg detected! - Start Hex: 0x2e000 - End Hex: 0x2f234 - Nr: 3
------> .jpg detected! - Start Hex: 0x30000 - End Hex: 0x326e4 - Nr: 4
------> .jpg detected! - Start Hex: 0x33000 - End Hex: 0x33e73 - Nr: 5
------> .jpg detected! - Start Hex: 0x34000 - End Hex: 0x362c0 - Nr: 6
------> .jpg detected! - Start Hex: 0x37000 - End Hex: 0x38b20 - Nr: 7
------> .jpg detected! - Start Hex: 0x39000 - End Hex: 0x3b7e7 - Nr: 8
------> .jpg detected! - Start Hex: 0xb7000 - End Hex: 0xb8234 - Nr: 9
------> .jpg detected! - Start Hex: 0xb9000 - End Hex: 0xbb6e4 - Nr: 10
------> .jpg detected! - Start Hex: 0xbc000 - End Hex: 0xbce73 - Nr: 11
------> .jpg detected! - Start Hex: 0xbe000 - End Hex: 0xc02c0 - Nr: 12
------> .jpg detected! - Start Hex: 0xc1000 - End Hex: 0xc2b20 - Nr: 13
------> .jpg detected! - Start Hex: 0xc3000 - End Hex: 0xc57e7 - Nr: 14
------> .jpg detected! - Start Hex: 0x338219 - End Hex: 0x339be0 - Nr: 15
------> .jpg detected! - Start Hex: 0x33a498 - End Hex: 0x33bc9b - Nr: 16

--> Carving for: .png


--> Carving for: .pdf

------> .pdf detected! - Start Hex: 0xb4000 - End Hex: 0xb618c - Nr: 1
------> .pdf detected! - Start Hex: 0x530000 - End Hex: 0x53018f - Nr: 2

--> Carving finished

###########################################################################################

Execution Time: 0.059799 sec
```


# License

MIT