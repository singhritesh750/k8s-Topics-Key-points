# secrets

1. It is used to store the external configurations.

2. It stores data in the "Base64 encoded" format in key:value pair.

3. It is used to store the data like credentials, certificates etc.

_`By default, k8s does not encrypt the data so we have to first encrypt it and then have to write inside the secrets.`_

Run the command in shell to encrypt the data:

```bash

echo -n [DATA_TO_BE_ENCRYPT] | base64

```
