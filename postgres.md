[If Postgresql is not working on WSL refer to](https://stackoverflow.com/questions/45437824/postgresql-warning-could-not-flush-dirty-data-function-not-implemented)

Start the postgresql service 
`sudo service postgresql start`

Enter into postgresql
`sudo su postgres`

Get to psql 
`psql -U postgres`

Change password
`\password <user>`
