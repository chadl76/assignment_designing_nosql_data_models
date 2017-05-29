# assignment_designing_nosql_data_models
I'll have one data model hold the SQL please

Chad Lucas

Basic

1.

Users {
	user_id: int,
	username: string,
	email: string,
	password: string,
	enable_profile: boolean,
	disable_profile: boolean,
	profile {
	  dob: date,
	  gender: string,
	  phone: int,
	  location {
	    city: string,
	    state: string,
	    zip_code: int,
	}
	description: string
}

}

Intermediate

1. Restaurant
{
  username: string,
  tables_available: int,
  reservation {
    time: date,
    name: string,
    phone: int,
    guests: int,
 }
  table {
    table_id: int,
    seats: int,
    reserved: boolean,
    time_available: date,
  }
}

2. University
   {
      userid: int,
      username: string,
      email: string,
      logged_in: boolean,
      semester {
        class {
          enrolled: boolean,
          name: string,
          grade: char, 
    
      }
   }

 Advanced

 1.