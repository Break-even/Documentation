# Git convention and practices

Here are the suggested git practices we recommend to follow to make the collaboration easy and free of pain.

## Issues

Label issues with the best fitting label. Keep the number of labels to a minimum but add or rename labels as needed.

Unlabeled issues might be considered dirty and uncategorized and might thus not be recognized among other labeled issues.

Use multiple labels to signify urgency, e.g `bug` & `urgent`,  `feature` & `soon`, or `question` & `later`.

When working on an issue, name the branch according to the issue id. E.g. `issue14-bugfix-duplicate-data`, `issue8-feature-sorting-by-company-name`

## Treat the master branch with care

No work in progress commits should be pushed on the master branch.

Bugs happen, but make sure that your merged version works before pushing to the master branch.

No `--force` anything on the master branch! This will surely create a mess for everyone when they want to synchronize their remote clone!

Please check your git diff for any unnecessary changes

## Version handling

Recommended is a version of [Semantic Versioning](https://semver.org/)

Tags are useful for version handling. Update the version number and push with the tag e.g `1.5.2` on the *master* branch. Any commits after that tag are considered snapshots of the next minor version e.g. `1.6.0-SNAPSHOT`. If it only contains patches, then specify the next patch version instead on release e.g. `1.5.3`.
