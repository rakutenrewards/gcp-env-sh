## gcp-env-sh

List runtime config/secrets from a gcp project in your shell.

### Install with brew

You need to set `HOMEBREW_GITHUB_API_TOKEN` env var as a GH token that has access to the RakutenReady organization.

Use the following command:

```
brew tap RakutenReady/gcp-env-sh git@github.com:RakutenReady/gcp-env-sh.git
brew install gcp-env
```

### Example usage

```
% ./gcp-env --project gcp-env-s1-5b4f
Listing environment from project gcp-env-s1-5b4f runtime configuration and secret manager
rr_gcpenvlib_runtime_config_text=rr_gcpenvlib_runtime_config_text_test
rr_gcpenvlib_runtime_config_value=rr_gcpenvlib_runtime_config_value_test
rr_gcpenvlib_secret_multiple_versions
rr_gcpenvlib_secret_single_version
```

### Source values

You may also run the following command if you desire to source these values:
```
% source ./gcp-env --project gcp-env-s1-5b4f --export
```
