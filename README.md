# release-playground
Hello!

Note:
* Test 1: Set the pre-release to false, and remove the versioning. Then remove the rc suffix from the `.release-please-manifest.json`
  * Outcome:
    * Didn't have to update the merge commit to use a feat/fix prefix. 
    * Bumps up the main version i.e., lets say the pre-release version was 3.1.0-rc, it bumps the version to 4.0.0
* Test 2: This removes the pre-release configs and also the -rc suffix from the `.release-please-manifest.json`
  * Currently, the version is 4.1.0-rc. Lets see what happens when we push this change & merge the changes.
  * Outcome:
    * Bumps the major version to 5.0.0
* Test 3: Create a pre-release
  * Outcome: Worked as expected and bumped up the minor
* Test 4: Removes the pre-release configs. Downs the version to 5.0.0 from 5.1.0-rc and removes the -rc lets see how it works. 
  * Also sets the `"bump-minor-pre-major": true,`
  * Outcome:
    * Expected outcome is to bring the release version up to 5.1.0