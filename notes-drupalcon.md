Security In Drupal Session
==========================
- first step : identify user input 
- most important vulnerabilities : XSS, Access Bypass
- CSRF :
	- eg a user places a img with src  user/delete/1 on ext.website 
    - form tokens avoid this. ( ensure that you  execute the action from the intended form )