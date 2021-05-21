# rails_github_action
Github action to deploy rails 6.1
- MySQL 5.7
- Ruby v3.0.0
- Node v14
- Redis

The main configuration is `.github/workflows/CI.yml`

So that databse.yml doesn't need to be edited, include config/CI_database.yml which is copied over the production database.yml on line 48 of the CI.yml file.

Tests are run at line 55. This is set up for minitest - change this line if you use something different.

Finally, rubocop is run at line 58.  Remove lines 57 and 58 if you don't use rubocop.