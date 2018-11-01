#Week 2 Day 4 Notes

### 1. Status Check & Recap Approach

Error drive development - using errors to control our development process

### 2. HTTP statelessness

Both sides are ignorant of eac other.
The protocol doesn't really save anything.

What is STATE?

 - Something having information that can be changed.
 - Peristen information
 - Memory

 - "The server has amnesia". It doesn't remember the browser

### 3. Statelessness without Cookies

HTTP Requests involve:

1. Verb
2. Path

Persistent Connection

Tracking users by IP address
 - They can be reassigned.

SCENARIO

    1. User goes to login page
    2. User fills in username and pwd
    3. Server confirms they are a user
    4. server redirects them to /prfile?username=[username]
    5. User makes a GET req to that URL
    6. Server extracts username from the URL
    7. Server renders profile.ejs with all <a> tags have `?username=[username]`

    Problems:

    1. Closing tab or open another to /profile, going to appear logged out. Tied to the session
    2. Spoofing by guessing: can pretend to be any user by guessing username
    3. Accidental spoffing by sharing of URL
    4. Sensitive information in the address bar is generally not advisable
    5. Potention for man in the middle attacak by snooping traffic data. HTTP vs HTTPS

### 4. Enter cookies

Cookies allow us to save client information on the client side and the client side sends it to the server with every request

One big difference with cookies is that the value is not in the URL and therefore hidden from plain view

Problesm solves: 1, 3, 4. Problem 2 is not solved, but it is harder to do.

### 5. Language Switcher Demo

### 6. User Authentication Demo

### 7. Other Security Implications