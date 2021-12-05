# post is japanese zipcode search program
command reference  
post <katakana yomi with %>  
'%' is all matching charactor  

## Make Env.
1.Create Database on postgresql vers version 10 or later.  
2.create zipcode_tbl  
psql dbname < zipcode_tbl  
3.edit postgresql.conf  
original  
lesten_address = 'localhost'  
change to  
lesten_address = '*'  
4.edit pg_hba.conf  
add last
host [database name] [user name] [network address]  ['password' or 'md5']
