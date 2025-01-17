## cast wallet new

### NAME

cast-wallet-new - Create a new random keypair.

### SYNOPSIS

``cast wallet new`` [*options*] [*path*]

### DESCRIPTION

Create a new random keypair.

If *path* is specified, then the new keypair will be written to a JSON keystore encrypted with a password.

### OPTIONS

#### Keystore Options

`-p`  
`--password`  
&nbsp;&nbsp;&nbsp;&nbsp;Triggers a hidden password prompt for the JSON keystore.

`--unsafe-password` *password*  
&nbsp;&nbsp;&nbsp;&nbsp;Password for the JSON keystore in cleartext.

&nbsp;&nbsp;&nbsp;&nbsp;This is **unsafe** to use and we recommend using `--password` instead.  
&nbsp;&nbsp;&nbsp;&nbsp;Environment: `CAST_PASSWORD`

{{#include common-options.md}}

### EXAMPLES

1. Create a new keypair without saving it to a keystore:
    ```sh
    cast wallet new
    ```

2. Create a new keypair and save it in `keystore.json`:
    ```sh
    cast wallet new keystore.json
    ```

### SEE ALSO

[cast](./cast.md), [cast wallet](./cast-wallet.md)
