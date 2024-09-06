# registry-creds operator Helm Chart
Due to the Docker hub rate limits introduction we need now to use authenticated requests to the Docker Hub registy (so far the only one having these limitatons).

To solve the issue we are making use the _registy-creds operator_ project: more info on its [Github page](https://github.com/alexellis/registry-creds).

The Docker hub credentials needed are stored in LastPass.

## Requirements

## Pre and Post install
No need of manual operations: Helm Hooks take care of creating the docker credendial secret necessary by the ClusterPullSecret this object itself.

