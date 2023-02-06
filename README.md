For Project Setup:

Clone repo.
Run [php artisan migrate] and [php artisan serve]


For testing:

Dashboard Test Suite
----------------------------------------------------------------
    - Not logged in yet
        - Click on the [Pokemon logo]
            - Should be redirected to welcome page(one with pokeball)
        - Click on Login
            - Should be redirected to login page
        - Click on Register
            - Should be redirected to register page

    - Logged in
        - Click on the [Pokemon logo] or [Pokemons] nav bar
            - Should see list of Pokemon and Welcome {Email}
        - Click on the [Account] nav bar
            - Should Welcome {Email} and User Info Form
        - Click on [My Likes] nav bar
            - Should see all liked Pokemon(if any, max 3)
        - Click on [My Hates] nav bar
            - Should see all hated Pokemon(if any, max 3)
        - Click [Other Users] nav bar
            - Should see list of other users(if any)
            - Should see own row as [This is Me!] for the username
----------------------------------------------------------------
Home Page Test Suite
----------------------------------------------------------------
    - Register
        - Click Register while all fields or 1 of them is blank
            - "Please don't leave blank" should prompt
        - Create user successfully
            - Should be redirected to login
        - Create the same email
            "Email taken!" should prompt
    - Login
        - Click Login while all fields or 1 of them is blank
            - "Please don't leave blank" should prompt
        - Login using unregistered email
            - "Unauthorized Login" should prompt
        - Login using registered email
            - Should be Redirected to [Pokemons] page

Note:

    - Fixed what I wanted to fix on the first source code I submitted.
    
    - Usually need 2-4 weeks to learn and adapt a new tech stach  
    but previous PHP experience and js frameworks experience helped
    in reading and understanding base source code.
