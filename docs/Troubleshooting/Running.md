
If you have not installed FreeTAKServer please follow the [installation](../Installation/platform/Linux/installation_vm) guide first.

## Run FTS in the Console

```bash
sudo python3 -m FreeTAKServer.controllers.services.FTS
```
If you have FTS running in the terminal how you like;
it is time to move on to running FTS as a [service](Service.md).

## Legacy Parameters
those parameters were supported in previous version of FTS

| Flag                | Default | Description                                                              |
|---------------------|---------|--------------------------------------------------------------------------|
| -AutoStart          |         | Weather the full server start or just the RestAPI, must be True or False |
| -CoTIP              |         | Your Server IP                                                           |
| -CoTPort            | 8087    | The port you want clients to connect to                                  |
| -SSLCoTIP           |         | Your SSL Server IP                                                       |
| -SSLCoTPort         | 8089    | The port you want SSL clients to connect to                              |
| -DataPackageIP      | 0.0.0.0 | The IP where data packages are served from                               |
| -DataPackagePort    | 8080    | The port you want Data Packages to be sent and received on               |
| -SSLDataPackageIP   | 0.0.0.0 | The IP where data SSL packages are served from                           |
| -SSLDataPackagePort | 8443    | The port you want SSL Data Packages to be sent and received on           |

