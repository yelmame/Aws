FSx:

prerequisites 
 domain registered name 
route 53 hosted zone 
create directory service for 2 subnet 
create FSX service foe windows  

Directory service in windows

step 1: directory service 
create AWS managed active directory 
standard edition 

step 2: select dns name (domain name which is registered in hosted zone )
grrasawstraining.online 

step3: give admin password 

select vpc & multiple subnet to have high availability 

step4 : it takes 30 -40 min 
 
step5: create fsx service for windows 

step 6: select standard create 
           name : filesystem: devops 
            security group as domain controller 
	   multi-az support  same subnet used in Directory service 
	   storage ssd: 32GB 
            
step 7: create 2 windows server in subnet we create in above steps 

step 8: login with windows server 
           go to network settting of each server in preferred & alternate dns server copy ip address of directoey service ip address 
step 9 : goto server system setting - about system 
	   member of : domain enter name :- grrasawstraining.online 
           after successfully join with domain 
step 10 :now go to directory service dns end point copy it and paste in 
            windows server -> this pc - \\directoery service dns end point of fsx(network& security)
            now can get share folder follow same procedure onn server2 
            create folder inn share folder from another server access from server1 



	



  