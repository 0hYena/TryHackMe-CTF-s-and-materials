# TryHackMe-CTF Neighbour 18.02.2026
On Try hack me i tried the Neighbour CTF and this is how it went

I was given the ip of 10.80.152.89 so i open the terminal and put in 
"nmap 10.80.152.89"
The results showed me 2 ports that were open, port 80 http and port 22 ssh. If we open firefox and put the IP address as the URL then we are sent to a page
<img width="753" height="589" alt="Screenshot_2026-02-18_11-49-34" src="https://github.com/user-attachments/assets/a2dc18a9-941c-4ca8-a61d-9de2e9f65a70" />

If we open the source code and see whats inside we are informed in the notes that are in green text that the guest account credentials are guest guest.
<img width="756" height="469" alt="Screenshot_2026-02-18_11-50-16" src="https://github.com/user-attachments/assets/6f569183-de96-4ee8-8151-24de57eb5e03" />
<img width="757" height="440" alt="Screenshot_2026-02-18_11-51-34" src="https://github.com/user-attachments/assets/987433ad-658e-4772-b1f1-8472e0245dbc" />

At the top of the URL i see that is said "=guest" so i though what if i try the defaults which is when you atempt to access something with common default credentials like admin, or password, this is a security risk if its the case as having predictable credentials puts the host of the website at risk.
<img width="754" height="328" alt="Screenshot_2026-02-18_11-51-57" src="https://github.com/user-attachments/assets/776cea56-394f-41e1-a300-96154195d56c" />

Voila! turns out this was the case and as we can see the Flag is in the screenshot.
