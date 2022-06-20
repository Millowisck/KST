# KST
Katalon Simple Test, testing login and logaout at https://ultimateqa.com/automation/
# SCRIPT 
Command	Target	Value
open	https://www.ultimateqa.com/automation/	https://www.ultimateqa.com/automation/
assertElementPresent	link=Login automation	
clickAndWait	//a[contains(.,'Login automation')]	
assertElementPresent	id=user[email]	
type	id=user[email]	testeroprogramowania1@gmail.com
verifyValue	id=user[email]	testeroprogramowania1@gmail.com
assertElementPresent	id=user[password]	
type	id=user[password]	oprogramowania
verifyValue	id=user[password]	oprogramowania
pause		2000
assertElementPresent	class=button button-primary g-recaptcha	value=Sign in
clickAndWait	class=button button-primary g-recaptcha	
assertElementPresent	class=header__mobile-button hidden-print	
click	class=header__mobile-button hidden-print	
click	link=Sign Out	
