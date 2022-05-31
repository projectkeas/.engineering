# Keas Engineering

This repo contains generic workflows and files that can be replicated across all repositories.

## Available Actions

Located under `.github/actions`

|Name|Description|Usage|
|---|---|---|
|docker-build|Performs a multi-architecture docker build, complete with caching|`uses: projectkeas/.engineering/.github/actions/docker-build@main`|
|go-build|Performs a multi-architecture golang build, complete with caching|`uses: projectkeas/.engineering/.github/actions/go-build@main`|
|publish-release-assets|Uploads specified assets to the current Github release|`uses: projectkeas/.engineering/.github/actions/publish-release-assets@main`|
|setup-supplychain-security|Installs [cosign]() alongside `anchore/syft` and `anchore/grype` to do supply chain security|`uses: projectkeas/.engineering/.github/actions/setup-supplychain-security@main`|

## Workflows

Located under `.github/workflows`

|Name|Description|
|---|---|
|copy-files-common|Copies files from the `files/common` to all listed repos in the matrix. This periodically needs checking to ensure the repository list is up to date.|
|copy-files-go|Copies files from the `files/go` to all listed repos in the matrix. This periodically needs checking to ensure the repository list is up to date.|
|label-sync|Ensures that labels are set correctly across all the repos. This periodically needs checking to ensure the repository list is up to date.|