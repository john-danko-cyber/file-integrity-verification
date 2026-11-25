# File Integrity Verification

These are hands-on labs on checking whether a file has been altered by comparing a hash I calculate against a known-good value. This repository will grow as I add more hashing and integrity labs. The first lab is a CompTIA Security+ course lab completed in Windows PowerShell.

## Labs

| Lab | What it covers | Key skills |
| --- | --- | --- |
| [Compare an MD5 Hash](md5-hash-comparison/) | Confirm a downloaded zip matches the vendor's published MD5 hash | PowerShell `Get-FileHash`, `Get-Content`, `-eq`, file integrity |

## Skills Demonstrated

- Generating a file hash with PowerShell `Get-FileHash`
- Reading a vendor-published hash with `Get-Content`
- Comparing hashes with `-eq` to verify integrity
- Using `-Algorithm` or `-a` because `Get-FileHash` defaults to SHA256
- Recognizing that a one-byte change produces a completely different hash
- Knowing that MD5 can detect accidental changes but is weak against deliberate collisions, so SHA256 is preferred

## Tools Used

- Windows PowerShell (course lab environment)
- `Get-FileHash` (MD5)
- `Get-Content`
