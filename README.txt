GEtiime README
by Daniel Yoachim

Overview
_____________________________________________
GEtime is an employee hours tracker. From the home page, create and account with login. When signed in, employees can update their name, username(which is used for the login), and password. 




To Create a new account
_____________________________________________
Create a new account from the add_worker path.
localhost:3000/add_worker


To Enable managaer status
_____________________________________________
Managers will be able to view all employees hour logs (Employees can only see their own). Managers can currently delete employees, which will remove all timesheets associated with them.

	Create the account you plan to change.
	rails console
	Employee.find_by_username(:username)
	Employee.toggle!.manager?


To Populate the database for testing purposes with FactoryGirl
_____________________________________________
	bundle exec rake db:migrate
	bundle exec rake db:populate
	bundle exec rake db:test:prepare


