# SQL-Injection-explanation


Lets do example for login system

table of username and password

when i login in any program that directly use database

when i enter my details on the website/program

the developer use `select query`

```sql
SELECT * FROM users WHERE username = writtenUsername AND password = writtenPasword
```

writtenUsername and writtenPasseord represent the username and password the user have entered in label fields

the gap here that you can comment the second condition **password condition**

by ending the username with sql comment label "--"

so for example we need to join accout with name "Allison" and i dont know its password so i will comment its password condition

username: Allison--
password: anythingItWIllBeCommentedAnyway

so the final replaced query label gonna be

```sql
SELECT * FROM users WHERE username = Allison-- AND password = anythingItWIllBeCommentedAnyway
```

As you see it will return the account without the password because password condition is commented as you see!
