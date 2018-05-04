# qualimap-multiqc-refinery-docker
Creates a Docker container wrapping MultiQC as a Refinery visualization.

## Development

After you checkout the repo you can build and run the docker container:
```
$ ./build.sh
$ ./run.sh good-input.json
```

Or you can run tests:
```
$ ./test.sh
```

## Release

Successful Github tags and PRs will prompt Travis to push the built image to Dockerhub. For a new version number:
```
$ git tag v0.0.x && git push origin --tags
```