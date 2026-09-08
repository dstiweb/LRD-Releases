# Windows Defender SmartScreen

Current LRD Beta executables do **not** yet have a commercial code-signing certificate and are therefore not digitally signed.

When an unsigned or newly published executable is downloaded from the Internet, Windows Defender SmartScreen may display a message similar to:

> Windows protected your PC  
> Microsoft Defender SmartScreen prevented an unrecognized app from starting.

This warning does not by itself mean that the file contains malware. SmartScreen also considers code signatures and file reputation, and a new unsigned build does not yet have established reputation.

## If you intentionally downloaded LRD from the official LRD release source

If Windows offers the normal SmartScreen override and you have verified that the file is the intended LRD download:

1. Select **More info** / **Weitere Informationen**.
2. Verify the displayed application/file information.
3. Select **Run anyway** / **Trotzdem ausführen**.

The wording can vary slightly between Windows versions and languages.

## Do not disable SmartScreen globally

LRD does not require Windows security features to be disabled. Do not globally turn off SmartScreen merely to run LRD.

Windows 11 Smart App Control, company security policies or administrator restrictions may completely block unsigned applications and may not offer a **Run anyway** option. In that case, follow the applicable security policy instead of weakening it solely for LRD.

## File verification

Public release packages should include a SHA-256 checksum file. It can be used to verify that the downloaded package matches the published release asset.
