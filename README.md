# test-refactor-code

-- this is the best approach as it allows us to seperate the business logic,application logic from controllers in to seperate php files and controller is just redirecting and seperating models from controllers also. In complex and large applications it gives us many benefits 
-less duplication of code           - central access to repetative tasks/functions
-less chances of errors

-- if we are going to send the push notification to user from multiple perspective then we can create a seperate file or we can include that piece of code in the helper file with static push notification function and use it in multiple files instead of writing same piece of code in multiple files.
--We can use ternary operator for shortening code instead of if/else.
-- While updating record we are first loading record from database then updating while we can directly update using the eloquent (basically performing one line query is good)
-- there is one function distancefeed in bookingcontroller where the all logic is in controller so we just moved that in to the bookingrepository and use from there.
So beside everything this is a good approach.