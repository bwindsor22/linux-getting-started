# Install Tmux
* `sudo yum install tmux`
* `tmux`
* `ctrl + B %`
* `ctrl + B "`

# Make directories and files
* `pwd`
* `whoami`
* `ls`
* `mkdir directory`
* `cd directory`
* `touch hi.txt`
* `ls`
* `mv hi.txt hello.txt`
* `ls`

# Edit a file with Nano
* `nano hello.txt`

# Vim
* `vimtutor`

# Htop
* `sudo yum install htop`
* `htop`

# Run sqllite table
* `sudo yum install sqlite-devel
* https://www.digitalocean.com/community/tutorials/how-and-when-to-use-sqlite 

# Load Real Data
* See https://perso.telecom-paristech.fr/eagan/class/igr204/datasets
* See https://docs.microsoft.com/en-us/dotnet/standard/data/sqlite/types
* wget https://perso.telecom-paristech.fr/eagan/class/igr204/data/cars.csv
* Replace all ; with , per this: https://vim.fandom.com/wiki/Search_and_replace
* sqlite3 database.db
CREATE TABLE cars(
  Car TEXT NOT NULL,
  MPG Double,
  Cylinders Double,
  Displacement Double,
  Horespower Double,
  Weight Double,
  Acceleration Double,
  Model TEXT,
  Origin TEXT
);

* .tables
* .mode csv
* .import /home/ec2-user/us-500.csv cars
* Run a sample query:
select *
from cars
where Origin == "US"


# Run a flask server
* https://flask.palletsprojects.com/en/2.1.x/quickstart/
* export FLASK_APP=hello
* flask run --host=0.0.0.0
* From another window: `curl -X get http://172.31.26.159:5000/` 

# Connect your python server to your database
* https://www.sqlitetutorial.net/sqlite-python/sqlite-python-select/


# Putting it together
* Write an endpoint in python that accepts an argument and prints a value
```

```
* Write an endpoint in python that accepts an MPG and returns the models which have at least the same MPG
* Write a curl call that triggers the response

# Extra Time? See "Missing Semester":
* https://missing.csail.mit.edu/ 

