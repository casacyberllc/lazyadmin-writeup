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

