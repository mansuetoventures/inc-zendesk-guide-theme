# Setup
1. https://develop.zendesk.com/hc/en-us/articles/360001075048
2. https://support.zendesk.com/hc/en-us/articles/115012793547-Previewing-theme-changes-locally-Guide-Professional-and-Enterprise-

# TL;DR Prerequisites
1. Have ruby installed, verify using `ruby -v`
2. `gem install rake`
3. `gem install zendesk_apps_tools`, to update, `gem update zendesk_apps_tools`

# Local Development
1. `zat theme preview`
2. Zendesk subdomain is: `incmagazine`
3. If using API token as password, username is: `jdoe@example.com/token`. Else, username is `jdoe@example.com`
4. Password is either API token or the Zendesk account password
5. Navigate to https://incmagazine.zendesk.com/hc/admin/local_preview/start
6. URL will change to https://incmagazine.zendesk.com/hc/en-us but sticky bar at the top will indicate "Help Center is in Preview mode"
7. Local changes will hot reload to reflect in the browser.
8. Push to remote master will not auto update the live theme. Navigate to https://incmagazine.zendesk.com/theming/workbench, Click the options menu on the theme with a Github icon, then select Update from GitHub. You need an admin zendesk account to do this.