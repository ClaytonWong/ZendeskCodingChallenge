# ZendeskCodingChallenge
Coding challenge for associate software engineer role

To do the coding challenge I had to take the following:

Step 1:
Go to https://www.zendesk.com/register/#getstarted to create Zendesk account.

Step 2:
Go to https://gist.github.com/svizzari/c7ffed8e10d3a456b40ac9d18f34289c

Step 3:
Save the contents of https://gist.github.com/svizzari/c7ffed8e10d3a456b40ac9d18f34289c as tickets.json

Step 4:
In a Linux terminal, type in the following:


curl -u c_w_serious-zendesk@yahoo.com:{password} https://claytonwong.zendesk.com/api/v2/imports/tickets/create_many.json  -v \

-X POST -d @tickets.json -H "Content-Type: application/json"


NOTE: {password} is the password for my Zendesk account.


Step 5:
Login to my Zendesk account to check if the 100 tickets from https://gist.github.com/svizzari/c7ffed8e10d3a456b40ac9d18f34289c
have been imported.
