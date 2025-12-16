DNS is a hierarchical and distributed naming system that translates domain names into IP addresses. When you type a domain name like "www.geeksforgeeks.org" into your browser, DNS ensures that the request reaches the correct server by resolving the domain to its corresponding IP address.

Working of DNS

The DNS process can be broken down into several steps, ensuring that users can access websites by simply typing a domain name into their browser.

<img width="926" height="442" alt="image" src="https://github.com/user-attachments/assets/6d5e7126-b0a1-48da-be5a-1b13da3fc026" />

User Input: You enter a website address (for example, www.geeksforgeeks.org) into your web browser.

Local Cache Check: Your browser first checks its local cache to see if it has recently looked up the domain. If it finds the corresponding IP address, it uses that directly without querying external servers.
<img width="926" height="442" alt="image" src="https://github.com/user-attachments/assets/323f2382-f21b-4044-a376-7ff392df7887" />

DNS Resolver Query: If the IP address isn’t in the local cache, your computer sends a request to a DNS resolver. The resolver is typically provided by your Internet Service Provider (ISP) or your network settings.
<img width="926" height="442" alt="image" src="https://github.com/user-attachments/assets/c9fbcf24-ae31-4722-81df-fef775701ea9" />

Root DNS Server: The resolver sends the request to a root DNS server. The root server doesn’t know the exact IP address for www.geeksforgeeks.org but knows which Top-Level Domain (TLD) server to query based on the domain’s extension (e.g., .org).
<img width="926" height="442" alt="image" src="https://github.com/user-attachments/assets/b185dd88-1160-45b5-92b2-c7e238f13fa7" />

TLD Server: The TLD server for .org directs the resolver to the authoritative DNS server for geeksforgeeks.org.

Authoritative DNS Server: This server holds the actual DNS records for geeksforgeeks.org, including the IP address of the website’s server. It sends this IP address back to the resolver.

Final Response: The DNS resolver sends the IP address to your computer, allowing it to connect to the website’s server and load the page.




