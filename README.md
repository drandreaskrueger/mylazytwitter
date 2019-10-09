# mylazytwitter
scripts to automate away boring tasks on twitter, probably using tweepy

# env
```
python3 -m venv ../../env/mylazytwitter
source  ../../env/mylazytwitter/bin/activate
pip install -U pip
pip install tweepy
pip3 install jupyter ipykernel
ipython kernel install --user --name="Python.3.mylazytwitter"
```

# run

    source  ../../env/mylazytwitter/bin/activate

## automated retweeting

    python retweeter_sleep.py
    
## show accounts in browser 
* who **retweeted** me recently
* who are not yet following me
* who are not in my "not interested" blacklist

    python retweets_examine.py | tee -a "../logs/$(date +%Y%m%d-%H%M)_retweets_examine.log"


