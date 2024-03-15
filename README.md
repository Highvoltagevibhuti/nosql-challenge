**Create NoSql database by importing establishment jason file into new uk_food database.**

Use following command inro gitbash:

mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json

mongosh

use uk_food

show collections.


