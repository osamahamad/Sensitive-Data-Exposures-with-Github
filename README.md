# Sensitive-Data-Exposures-with-Github
Techniques / Tips and tricks for finding sensitive data exposures in Github for Penetration Testers / Bug Bounty Hunters 



https://www.youtube.com/watch?v=l0YsEk_59fQ 

Inspired by @Th3G3nt3lman

## Find Sensitive information leaks : ( Manual Approch ) 

Below basic examples : 

"Company" password 

"Company" secret 

"Company" credentials 

"Company" token 

"Company" config 

"Company" key 

"Company" pass 

"Company" login

"Company" ftp

"Company" pwd

"Company" vspher

"Company" aws

"Company" jenkins





With creaitivity there is a lot of stuff to look for : 

"Company" security_credentials    ---> LDAP ( active directories ) 

"Company" connectionstring    ---> Database Cred

"Company" JDBC ---> Database Cred

"Company" ssh2_auth_password ---> unautorized access to servers 

"Company" send_keys 

"Company" send,keys

"Company" ldap


List of keywords , much thanks : 

https://github.com/random-robbie/keywords/blob/master/keywords.txt

https://securitytrails.com/blog/github-dorks


________________________


You can use language:python for example to search for specific programing language codes. Example : 

"Company" language:pyhton password 


________________________


From [ Sort ] , you can use it to find for [ Recently Indexed ] ones which is important.

________________________


"Company" language:pyhton password NOT owner-api.teslamotors.com 

Will sort the results and remove everything realted to  [ owner-api.teslamotors.com  ] 


________________________


user:VALUE ---> To look for code commited for a specific user

org:Value ---> Specific org 








## Find Sensitive information leaks : ( Automation Approch ) 


Using gitrob : https://github.com/michenriksen/gitrob

Using TruffleHog : https://github.com/dxa4481/truffleHog

Using gitGraber: https://github.com/hisxo/gitGraber

Using git-all-secrets: https://github.com/anshumanbh/git-all-secrets

Using Truffle hunting: https://github.com/dxa4481/truffleHog


https://github.com/gwen001/github-search

Don't forget bitbucket, gitlab and google dorking 2.
https://lmgtfy.com/

