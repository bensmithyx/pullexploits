# pullexploits

This code will run the command $sudo -l on a linux system. From the results it will webscrape [GTFObins](https://gtfobins.github.io/) for exploits. It will then download the exploits found into a bash file to be run via a cli menu.

# Usage

`python3 pullexploit.py`

Long argument | Short argument | Value                 
------------  | -------------  | -------------
--help        | -h             | n/a
--option      | -o             | [check\|findexploits\|offlinetarget\|offlinehost\|runexploits]
--verbose     | -v             | n/a 

# Machine with internet

First time run
`python3 pullexploits.py -o findexploits`

Once exploits folder has been created
`python3 pullexploits.py -o runexploits`

# Machine without internet

On machine with interent
`python3 pullexploits.py -o offlinehost`

On machine without internet
`python3 pullexploits.py -o offlinetarget`

# Check if there is a valid exploit

`python3 pullexploit.py check`

returns True or False
