# Release Notes


## What's new in release 2020-11-25

### :rocket: Improvements

- Updated advice on Email Traffic IPs page

- Updated advice on SPF lookup advisories

- Removed 'Beta' badge

- Notifications now available for TLS changes

- Display familiar names for popular email providers

### :bug: Fixes

- Fix for CSV export

- DMARC advisories use `sp` field correctly


## What's new in release 2020-10-22

### :rocket: Improvements

- Manage workspaces page will now show domain verification type

- Added a dedicated "Add Subdomain" button to domain summary page

### :bug: Fixes

- 


## What's new in release 2020-10-21

### :rocket: Improvements

- A user is now able to delete or rename a workspace

- Additional guidance added to email traffic IPs page

- Removing incorrect "alert" role from frontend message boxes

### :bug: Fixes

- 


## What's new in release 2020-10-19

### :rocket: Improvements

- A user is now able to remove domains from their workspaces

- Clarified wording around partially trusted emails still passing DMARC checks

### :bug: Fixes

- Fixed an issue with the "Check Now" button

- Fixed a number of issue with the TLS configuration tester


## What's new in release 2020-10-09

### :rocket: Improvements

- Improved test coverage for SPF

- Amended outdated DMARC advice 

### :bug: Fixes

- Amending DMARC parsing to allow colon separated list of failure options

- Amending DMARC record instructional text to include missing semi-colon


## What's new in release 2020-10-02

### :rocket: Improvements

- Removing duplicated logging in DNS clients

- Amended database migration scripts to run GRANTs on every deployment

- Auto-generating database user passwords if missing

### :bug: Fixes

- Fixed null reference bug in SPF
