gulp-release-it
=============

Provides an automatic way to do a release of your npm modules to Git and publish it to NPM Repository.

## Usage
`npm install gulp-release-it --save-dev`

```javascript
var gulp = require('gulp');
require('gulp-release-it')(gulp);
```

## How it works

1. Create a tag based on version specified in package.json
2. Publish the project to NPM repository 
3. Bumps the version of package.json, bower.json or/and manifest.json

## How to release (publish to NPM repo and GitHub)

```gulp release```

## How to bump and then release (publish to GitHub)

```gulp bump-release```

## How to release only to GitHub

```gulp github-release```

## How to release from different folder

```gulp release --rootDir=/path/to/project```

## Different ways to bump the version after release

command              | version
---------------------|-----------------
gulp release         | v0.0.1 -> v0.0.2 
gulp release --minor | v0.0.1 -> v0.1.0 
gulp release --major | v0.0.1 -> v1.0.1
gulp release --alpha | v0.0.1 -> v1.0.1-alpha.0
gulp release --beta  | v0.0.1 -> v1.0.1-beta.0
gulp release --RC    | v0.0.1 -> v1.0.1-RC.0

### If you want only to bump the version

command              | version
---------------------|-----------------
gulp bump            | v0.0.1 -> v0.0.2 
gulp bump --minor    | v0.0.1 -> v0.1.0 
gulp bump --major    | v0.0.1 -> v1.0.1
gulp bump --alpha    | v0.0.1 -> v1.0.1-alpha.0
gulp bump --beta     | v0.0.1 -> v1.0.1-beta.0
gulp bump --RC       | v0.0.1 -> v1.0.1-RC.0
 
## How to release from different branch
 
```gulp release --branch=branch_name```

