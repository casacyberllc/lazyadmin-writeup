# lazyadmin-writeup

<img width="1150" height="267" alt="image" src="https://github.com/user-attachments/assets/4cb001c3-8fc6-4d71-abcc-b5771ef90b7e" />

I checked the site, and it doesn't have anything telling. I'm going to use nmap to scan the open ports and see what services are running. 

<img width="889" height="524" alt="image" src="https://github.com/user-attachments/assets/d74c0905-bcf8-4b76-b9c4-9f21a59c4db8" />

I see ports 22 and 80 are open. Since 80 is open, it should have a webpage. Let me see if I can use gobuster to see what directories are listed. 

<hr />

<img width="914" height="426" alt="image" src="https://github.com/user-attachments/assets/f611e3b8-efc6-4ecb-bef3-ede83a7f31c7" />

Ok I see the content/ directory has additional directories 

Let's do another gobuster to see what is hiding beyond that. 

<img width="1015" height="494" alt="image" src="https://github.com/user-attachments/assets/090f3cf4-7762-4018-a68f-713032ab3756" />

We got a few things going there. I'm going to poke around to see what else I'm able to find. 

I'm drawn to the inc directory. Let's look around there. 

It just has a bunch of php files in it. Let's look around some other directories. Let's look at the /as directory. 

This takes me to a login page of some sort. 

<img width="538" height="589" alt="image" src="https://github.com/user-attachments/assets/e222ae38-7245-44c6-adff-d924b808ac0b" />

I'm not sure where this leads. Lets first check the source code for any hidden notes, then use gobuster to see what directories go past this. 

Ok using a login that doesn't match in their system leads to 'Login failed' as a response. Good to note before we try to brute force it. 

Let's use gobuster first to see what lies past this before we do anything more. 

<img width="1048" height="422" alt="image" src="https://github.com/user-attachments/assets/d2e21c94-20aa-4e0e-a3f5-8c3a3a13dbb1" />

It looks like there's a few pages we can look into. Let's check JS. 

I get access to it right away and see this. 

<img width="596" height="401" alt="image" src="https://github.com/user-attachments/assets/7852b45e-c2b2-4084-b82d-fc6ea13a4b9a" />


