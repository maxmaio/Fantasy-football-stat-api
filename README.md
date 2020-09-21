# Fantasy Football Stat API

This program will help you pull data from your yahoo fantasy football league.

## Requirements

- Python  3
- Jupyter
- Yahoo developer accout
- pandas
- [yahoo_oauth](https://pypi.org/project/yahoo_oauth/)
- Numpy
- Seaborn
- Matplotlib

## Guide to getting started

 1. Enter your League ID in the `league_info_form.txt`
 2. Update `league_info_form.txt` to include all details of your league
 3. Register as a yahoo developer at [https://developer.yahoo.com/](https://developer.yahoo.com/) --> 'My Apps' --> 'YDN Apps'
 4. click `create an app`
 5. Select the 'Installed Application' option since we're only going to be accessing the data from our local machines.
 6. Under the 'API Permissions' sections select 'Fantasy Sports' and then make sure that 'Read' is selected.
 7. You have now successfully created a Yahoo Developer App and you will see  `App ID`,  `Client ID(Consumer Key)`, and  `Client Secret(Consumer Secret)`  with a long string of random letters and numbers. Yahoo will use these keys to allow you to access it's API via OAuth 2.0.
 8. in directory `./auth`, open `oauth2yahoo.json`
 9. copy in `Consumer Key` and `consumer secret key` 
 10. run `leauge_authorization.py` 
 11. now you should be able to run `fantasy_stats.py`
 12.  run `data transformations.py` to output to csv
