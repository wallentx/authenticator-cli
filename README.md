# authenticator-cli

A commandline Authenticator App (for Authy, Google Authenticator, Microsoft Authenticator, Facebook Authenticator, TOTP, etc)

**Install node.js 4.0+**:

```bash
curl -L https://bit.ly/iojs-min | bash
```

**Install authenticator**:
```bash
npm install --global authenticator-cli
```

```
Usage:
  authenticator [OPTIONS]

Options:
      --account user@example.com    Account Name, typically email address (Default is user@example.com)

      --algo SHA1                   Algorithm, typically SHA1 (also SHA256, SHA512)  (Default is SHA1)

      --digits 6                    Number of digits, typically 6 (also 8) (Default is 6)

      --generate                    Create a cryptographically-random TOTP key
                                    formatted in base32 with spaces.  (Default is true)

      --issuer ACME                 Issuer, typically the company name (Google,
                                    Facebook, Digital Ocean, etc)  (Default is ACME)

      --key 'xxxx xxxx ...'         Supply the base32 key yourself (with or without
                                    delimeters). Takes precedence over --generate

      --period 30                   Number of seconds between tokens, typically 30  (Default is 30)

      --qr                          Print the QR Code to the Terminal.

      --verify '123 456'            Verify a token. Must be used with --key.

  -h, --help                        Display help and usage details
```
