# lms-update

## Description
A Bash script to update wtc-lms

## Setup
**NB** lms-update requies [slack-cli](https://github.com/regisb/slack-cli) to run.

1. Run `pip install slack-cli` to install slack-cli.
2. **Get your slack user token for `slack-cli`**:
  *Go to [slack customization page](https://my.slack.com/customize)
  * Open developer tools on your browser.
  * Go to the console and enter: `window.prompt(TS.boot_data.api_token)`
  * You should see a token string **xoxs-BUNCH-OF-NUMBERS**
  * Copy the token string.
3. Next you need to define the `SLACK_TOKEN` & `WTC_LMS_DIR` environment variables.
  * **SLACK_TOKEN** is required by slack-cli
  * **WTC_LMS_DIR** is the directory where the wtc-lsm binary will be stored.E.g. export WTC_LMS_DIR=`~/bin/wtc-lms`
5. Put following in your **.bashrc/.zshrc**:
* `export SLACK_TOKEN=xoxs-BUNCH-OF-NUMBERS`
* `export WTC_LMS_DIR="~/bin/wtc-lms"`

## TODO
Integrate this script with crontabs for auto-update functionality
