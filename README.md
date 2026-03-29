# HavokSDKTools
Havok Asset tool using all SDKs heavily inspired off assetcc2.

## What It Does

- Loads HKX packfiles across multiple Havok SDK generations.
- Handles Big Endian layout HKX files `550`, `2010_2_0_r1`, and `2012_2_0_r1` workflows in mind.
- Converts to XML or binary HKX output.
- Supports metadata stripping, custom layout rules, and user tag output.

## Supported Versions (x86)

- `550`
- `600`
- `650`
- `660`
- `710`
- `2010_2_0_r1`
- `2011_1_0_r1`
- `2011_2_0_r1`
- `2011_3_0_r1`
- `2012_2_0_r1`
- `2013_1_0_r1`
- `2013_2_0`
- `2014_1_0_r1`


## Usage

```text
AssetContentCompiler [options] Myinput MyOutput
```

### Options

- `-h`, `--help` Show help
- `-x`, `--xml` Write XML output (default)
- `-s`, `--strip` Strip metadata from output
- `-r`, `--rules####` Write binary using layout rules (`[48][01][01][01]`, example `4101`)
- `-t`, `--tagVALUE` Set userdata tag (decimal or hex, e.g. `0x1234`)
- `-v`, `--verbose` Increase verbosity (repeat for more)
