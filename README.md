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

 1. eCommerce
  {
    product_id: int,
    quantity: int,
    product_info {
      name: string,
      description: string,
      dept: string,
    }
    reciept {
      product_id: int,
      quantity_sold: int, 
    }
  }


 2. Activity Feed

 	{
 	user_id: int,
 	user_name: string,
 	profile {
 	  name: string,
 	  email: string,
 	  dob: date,

 	}
 	friends: array,

 	posts {
 	  post_id: int,
 	  name: string,
 	  body: text,
 	}
 	comments {
 	  comment_id: int,
 	  post_id: int,
 	  body: text

 	}

 	}