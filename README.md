form employees
{
	displayname = "Employees"
	success message = "Data Added Successfully!"
	Section
	(
		type = section
	 	row = 1
	 	column = 0   
		width = medium
	)
	employee_id
	(
    	type = autonumber
		displayname = "Employee ID"
		start index = 1
	 	row = 1
	 	column = 1   
		width = medium
	)
	full_name
	(
    	type = name
		displayname = "Full Name"
     	prefix
     	(
	     	 type = prefix
	     	 displayname ="Prefix"
	     	 visibility = false
	     	 value = {"Mr.","Mrs.","Ms."}
     	) 
     	first_name
     	(
	     	 type = first_name
	     	 displayname ="First Name"
     	) 
     	last_name
     	(
	     	 type = last_name
	     	 displayname ="Last Name"
	     	 visibility = false
     	) 
     	suffix
     	(
	     	 type = suffix
	     	 displayname ="Suffix"
	     	 visibility = false
     	) 
	 	row = 1
	 	column = 1   
		width = medium
	)
	job_title
	(
    	type = text
		displayname = "Job Title"
	 	row = 1
	 	column = 1   
		width = medium
	)
	department
	(
    	type = text
		displayname = "Department"
	 	row = 1
	 	column = 1   
		width = medium
	)
	hire_date
	(
    	type = date
		displayname = "Hire Date"
		alloweddays = 0,1,2,3,4,5,6
	 	row = 1
	 	column = 1   
		width = medium
	)
	email
	(
    	type = email
		displayname = "Email"
	 	row = 1
	 	column = 1   
		width = medium
	)
	phone
	(
    	type = phonenumber
		displayname = "Phone"
	 	row = 1
	 	column = 1   
		width = medium
	)
	manager
	(
    	type = text
		displayname = "Manager"
	 	row = 1
	 	column = 1   
		width = medium
	)
	
	actions
	{
		on add
		{
			submit
			(
   				type = submit
   				displayname = "Submit"
			)
			reset
			(
   				type = reset
   				displayname = "Reset"
			)
		}
		on edit
		{
			update
			(
   				type = submit
   				displayname = "Update"
			)
			cancel
			(
   				type = cancel
   				displayname = "Cancel"
			)
		}
	}
}
