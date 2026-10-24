# ABAJ Monitor publication

1. Build and verify the signed APK in the private source repository. Preserve package name and the existing signing certificate. Save QA files and base64 parts in the source branch; Actions artifact storage is not required.
2. Copy only the APK transfer parts into the public staging branch using an authorized GitHub connection. A repository-scoped GITHUB_TOKEN does not transfer files between these repositories. No additional PAT is required when using the existing connected GitHub access.
3. Complete all parts before launching publication. Reconstruct the APK and verify its byte count and SHA-256. Commit the complete staging set atomically.
4. Prepare the version-specific release workflow from release-monitor-076.yml: pin the verified staging commit, update version, paths, expected hashes and predecessor checks. The workflow uses contents: write with its own public-repository GITHUB_TOKEN.
5. Trigger publication by committing its release-ready marker only after staging verification. Verify signature, package and both Android version fields; publish APK files first, download and verify both public files, then update peer-updates.json.
6. Confirm the Actions run succeeded and independently download the exact manifest URL and APK URL. Keep all previous APKs. Do not regenerate an APK after fixing its published SHA-256.

The 0.7.6 source build previously compiled and committed successfully but failed at the redundant upload-artifact step because artifact storage quota was exhausted. That step has been removed from build-abaj-monitor-076.yml. The alternative direct cross-repository publisher is absent from the current source branch; it failed because ABAJ_MONITOR_RELEASE_TOKEN was unset. The original public publisher failed because staging was missing when it ran. Publication must never be triggered before staging is complete.
