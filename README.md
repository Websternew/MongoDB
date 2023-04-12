# MongoDB
 Create a new database called 'TripCollaborator'
        
        use trip_collaborator

 Create a collection called 'users'
      
      db.createCollection('users')

 Define the schema for the 'users' collection
      
      db.users.insertOne({
     username: "string",
     email: "string",
     password: "string",
     trips: [{
      trip_id: "string",
      role: "string"
     }]
     })

 Create a collection called 'trips'
     
     db.createCollection('trips')

 Define the schema for the 'trips' collection
      
      db.trips.insertOne({
      name: "string",
      start_date: "date",
      end_date: "date",
      location: {
        address: "string",
        city: "string",
        state: "string",
        country: "string"
       },
       expenses: [{
       amount: "float",
       user_id: "string"
       }],
    })
   Create a collection called 'location'
   
       db.createCollection('location');
   
   Define the schema for the 'location' collection
       
         db.location.insertOne({
         name: "string",
         trip_id:"string",
         start_date: "date",
         end_date: "date"
        })
