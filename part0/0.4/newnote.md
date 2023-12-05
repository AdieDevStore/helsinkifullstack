USERAGENT:  browser, Chrome
SERVER: studies.cs.helsinki.fl/exampleapp/notes, server: NodeJS

** ON PAGE LOAD **

USERAGENT calls SERVER and receives notes.html from SERVER
USERAGENT renders HTML
USERAGENT calls for main.css from SERVER and renders CSS formatting
USERAGENT calls for main.hs from SERVER

USERAGENT calls data.json using GET request to SERVER/exampleapp/data.json
USERAGENT renders data to body of HTML page
USERAGENT builds and renders input form, form POSTS to "exampleapp/new_note"

** ADD A NOTE ** 
USERAGENT receives text input from user
User clicks "save", payload is set and POST call sent to "exampleapp/new_note"
SERVER receieves request and sends 302 redirect code to USERAGENT
USERAGENT repeats steps from ** ON PAGE LOAD ** 