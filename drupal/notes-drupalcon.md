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

[Selling to large enterprises](http://munich2012.drupal.org/program/sessions/selling-drupal-web-experience-management-large-enterprises-choose-your-battles-and)
===========================================================================
by Felipe Rubim chief architect @ Ciandt ( active in US, China and Brasil )

- you have to keep selling Drupal within the enterprise
- Drupal sales team <> "other" sales team

"The Drupal community should build muscles & strategies"
- Do your howework

What is a "large enterprise"?
----------------------------
- have legacy systems
- have several integration points with other systems
- Global reach
- Several Groups involved 

Drupal's Selling points :
----------------
- flexibility
	- different approaches
- high innovation rate

Thing's that will improve in a short timeframe :
------------------------------------------------
- improved content authoring ( became more important in the last years )
- Site preview

FUD :
-----
- no support !
-> there's plenty of companies that provide support
- security
-> depends on the development team
-> no 100% secure solutions exist

Advantage:
----------
- you can influence the Drupal Roadmap ( company can become a member )

Understanding Web Experience Mgmt
----------------------------------
Marketing departments become more important, they're interested in knowing how Drupal can help to build their brand.

Tips :
------
- build a requirements score
- understand the business gap between IT & Marketing
- make sure you have demos

Panel Selling to large Enterprises:
===================================
What is enterprise?
-------------------
- more documented processes

Different roles in the sales departement:
-----------------------------------------
- marketing monitoring of twitter
- sales engineers contact leads

bottom-up <> bottom down approach

Tips :
------
- know your product, provide value during sales person.
- technological knowledge is key.
- Find someone who will be your advocate
- having enough people is important ( reason for the wunderkraut merge )
- Things that smaller shops forget :
	- enterprises don't want to give references
    - fees for exceeding deadlines
    - failure is not acceptable
- build a relationship -> finding the right people is key
- Bring demos! Drupal is fast to build smth, use this!
  ( but make sure it's worth the risk )
  

Continous Integration with Drupal
=================================
- big features -> small steps
- automate the upgrade process
- _" if it isn't tested it doesn't work "_
- start small, refactor later
- run tests frequently
- Test in a clone of production
- you should be able to fully trust this process
- _" CI is an attitude, not a tool "_
- drush is your friend
	- code
    - files
    - database ( sql-sync )
    
    






    





    