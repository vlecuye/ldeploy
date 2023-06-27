Looker Deployer makes use of the Looker SDK to communicate with your Looker instances. A looker.ini file is required to provide authentication. By default the tool looks for this file in your working directory but if it is named differently or in a different location you can make use of the --ini argument to specify its location. Here's an example ini file:

[dev]
base_url=https://looker-dev.company.com:19999
client_id=abc
client_secret=xyz
verify_ssl=True

[prod]
base_url=https://looker-prod.company.com:19999
client_id=abc
client_secret=xyz
verify_ssl=True

To create credentials, go to your looker instance. In the admin section, go to Settings, then Users. Find your user and click on it. You can then go to the API key section (under Edit Keys) and create a new key. This key will let you make looker deployer calls.