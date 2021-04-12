# Auto Github Bio

Auto Github bio using api of openweathermap.org.

https://prnt.sc/11aeift

## Installation

### [Github] Create your personal access token

You have to create a **personal access token**, to allow your app to update your biography. Click [here](https://github.com/settings/tokens/new) to go to the personal access token creation page. Select the `User` field (Update all user data) and click `Generate new token`. Copy and paste it in your **config.json** file (`github` field).

### [OpenWeatherMap] Get application key

You have to get your **openweathermap.org api key**, to allow your app to get the weather of your favourite city. Register [here](https://openweathermap.org/home/sign_up), then go on [dashboard](https://home.openweathermap.org/api_keys) to get your key. Copy and paste it in your **config.json** file (`weather` field).

### [Crontab] Run the script every 5 minutes

You have to edit the **crontab table** using `crontab -e`. Then, add the following line to this file:  
```sh
*/5 * * * * cd /path/to/auto-github-bio && /usr/bin/python3 /path/to/auto-github-bio/main.py >> ~/cron.log 2>&1
```
This will run the script and update your bio every 5 minutes.

### That's it

Congratulations, you have successfully installed Auto Github Bio. Feel free to open an issue if necessary!
