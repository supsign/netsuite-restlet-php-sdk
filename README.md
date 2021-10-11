# General
This is a Fork from Supsign GmbH to use this package with PHP 8.0. It depends on the improvement of the forked package if we some day open an Pull-Request.

# Setup
PHP 8.0+ compatible

## Symfony 3.4+
- Run `composer require infostud/netsuite-sdk:^2`
- Add a JSON config file based on [sample](sample.config.json)
- Set the path to that file in `NETSUITE_CONFIG_PATH` environment variable
- Register the service definition in your `services.yml`
```yaml
Infostud\NetSuiteSdk\ApiService:
    arguments:
        - '%env(NETSUITE_CONFIG_PATH)%'
```
