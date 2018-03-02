This template executes a combo of commands to create a domain registration request 
with a new owner contact
Lines marked with (optional) can be removed. If used you need to remove “(optional)”.

----templatestart
mailtemplateversion.....: 2.0
agreementsaccepted......: YES

command[1]..............: Login
API-key.................: 

command[2]..............: CreateContact
firstname...............:
lastname................:
organization............:
orgnr...................:
address1................:
zipcode.................:
city....................:
countrycode.............:
phone...................:
Fax.....................: (optional)
email...................:

command[3]..............: create-domain-registration
domainname..............: domain.com
itemyear................: 1
Ownerid.................: command[2]
Autorenew...............: (optional)
Shieldwhois.............: (optional)
Trustee.................: (optional)
Tmchacceptance..........: (optional)
Nameserver...........: (optional)
----templateend






This template executes a combo of commands to create a domain registration request with a existing owner contact

----templatestart
mailtemplateversion.....: 2.0
agreementsaccepted......: YES

command[1]..............: Login
API-key.................: 

command[3]..............: create-domain-registration
domainname..............: domain.com
itemyear................: 1
Ownerid.................: 123456789
Autorenew...............: 1
Shieldwhois.............: 0 
Trustee.................: 0
Tmchacceptance..........: 0
Nameserver...........: ns1.nameisp.info,ns2.nameisp.info
----templateend
