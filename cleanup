#!/bin/bash

# exit when any command fails
set -e

cd "${0%/*}"

git remote remove origin
git checkout --orphan newBranch
rm src/.gitignore
git add -A  # Add all files and commit them
git reset -- "$0"
git commit -m "Initial commit"
git branch -D master  # Deletes the master branch
git branch -m master  # Rename the current branch to master

echo "Done!"
rm -- "$0"
