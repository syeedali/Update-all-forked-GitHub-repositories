# DO NOT FORK THIS BLINDLY

Re-synchronizes AND OVERWRITES all forks throughout your GitHub account.

Also bulk-disables all automation of forks, because GitHub has no feature to do that easily.

BE AWARE:  If you intend to use the account in which this is running, to have forks which you contribute to, even if to work and then push a patch, then you must add an exception to the sync.yml herein or it will be overwritten.

You have to set up the appropriate permissions for this workflow:

- Set up a personal access token:  https://github.com/settings/tokens
- Scopes:
    - `repo` [all]:
    -  - `repo:status`
     - - `repo_deployment`
     - - `public_repoAccess`
     - - `repo:inviteAccess`
     - - `security_events`
  - `workflow`
