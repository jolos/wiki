[Security In Drupal Session](http://munich2012.drupal.org/node/733)
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
    
Functional PHP
==============

Procedural programming
-----------------------
 procedure = reusable series of commands

Declarative programming
-----------------------
You don't say how the code should be executed. But what it should do.
( e.g.  SQL )

Functional Programming
----------------------
- pure functions
- higher-order functions / first-class functions
- immutable variables
- recursion 

Advantages:
- no side-effects
- explicit function input/output
- stateless
- testability



    