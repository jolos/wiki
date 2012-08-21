Security In Drupal Session
==========================
- first step : identify all user input 
- most important vulnerabilities : XSS, Access Bypass
- CSRF :
	- description : eg a user places a img with src  user/delete/1 on ext.website 
    - solution : form tokens avoid this. ( ensure that you  execute the action from the intended form )
- XSS :
	- in-browser
    - hijacks the cookie of an authenthicated user
    - solution : validate input, use drupal API
    - check_url > check_plain > check_markup > filter_xss
- automated review :
	- security_review
    - hacked
    - coder
    - secure_code_review
    - http://github.com/unn/vuln 
    - http://drupalscout.com/node/11

    