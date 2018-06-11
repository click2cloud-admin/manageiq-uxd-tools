# manageiq-uxd-tools
Setup, maintenance and tampering tools to abstract away the ManageIQ API and help UX developers stick to what they do best.

## TODO

* Set up lerna packages:
  * setup - Run this once to install all deps or update them, and run all the ruby and webpack build stuff. this will be a port of my work from [miq_mac_dev](https://github.com/mturley/miq_mac_dev) but using rbenv instead of rvm, and with more sanity checking, and linux friendly.
  * debug - This will be a package you can import in your React code and pass things to, in order to get some hopefully helpful information in your console. You must remove it before merging a PR... don't worry, it will tell Travis to remind you.
  * tamper - This will be an HTTP Proxy Server that snoops on your local API traffic, and messes with the responses (when you tell it to). Helpful to scratch those itchy edge cases.
  * db - This will be a little CLI designed to help you swap between local `vmdb_development` databases and share database rows with others. Want to look at someone's branch? Look at their DB too, versioned along with the PR. I plan to start with some local postgres helpers, then maybe leverage Git LFS for the database backup storage if we get to the sharing part.
* Get back to work on the things that frustrated me enough to make this repo
