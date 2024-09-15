# release-playground
Hello!

Note:
* Test 1: Set the pre-release to false, and remove the versioning. Then remove the rc suffix from the `.release-please-manifest.json`
  * Outcome:
    * Didn't have to update the merge commit to use a feat/fix prefix. 
    * Bumps up the main version i.e., lets say the pre-release version was 3.1.0-rc, it bumps the version to 4.0.0