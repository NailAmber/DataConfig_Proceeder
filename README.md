# Python Script for Processing API Credentials
## Overview

This Python script reads phone numbers, API IDs, and API hashes from three separate text files located in the data directory. It processes these files line-by-line, matching each phone number with its corresponding API ID and API hash, and outputs a single file that can be used in other applications.
## Features

 - Reads data from three separate text files:
     - raw_numbers.txt for phone numbers
     - raw_api_id.txt for API IDs
     - raw_api_hash.txt for API hashes
 - Combines the data into a single output file
 - Easy to integrate with other Python applications

## Installation

  Clone the repository:

    git clone https://github.com/NailAmber/DataConfig_Proceeder.git
    cd DataConfig_Proceeder

  Ensure you have Python 3.x installed on your system.

## Usage

   Place your raw_numbers.txt, raw_api_id.txt, and raw_api_hash.txt files in the data directory.

   Run the script:

    python main.py

  The script will generate a api_config.json file in the main directory.

## Example
Input Files

  raw_numbers.txt:

```
+1111
+2222
+3333
+4444
```
raw_api_id.txt:
```
111111111
22222222
3333333333
4444444444
```
raw_api_hash.txt:

    abcdef123456
    654321fedcba
    123abc456def

Output File

  api_config.json:
```json
 {
    "+1111": [
        111111111,
        "aaaaaaaaaaa"
    ],
    "+2222": [
        22222222,
        "bbbbbbbbbbbb"
    ],
    "+3333": [
        3333333333,
        "cccccccccccc"
    ],
    "+4444": [
        4444444444,
        "dddddddddddd"
    ]
}
```
