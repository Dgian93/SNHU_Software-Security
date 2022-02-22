# SNHU_Software-Security
Repository for a Vulnerability Report Assessment Project for my software security class.

•	Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

Artemis Financial was a financial consulting company responsible for creating individualized plans in savings, retirement, insurance and investments for their customers. They tasked us to modernize their web application by first assessing current security vulnerabilities in their REST API – based web application and then implementing solutions to address those vulnerabilities.

•	What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

What I did well was to identify areas where Artemis’s web app needed more security measures. The first was that two server endpoints received user input but lacked any input validation. I also found in 2 different classes that public variables were being used for class members (which should be private) and therefore needed to be correctly encapsulated.  I also felt I did a decent job summarizing some of the known vulnerabilities from the dependency check report. It’s important to code securely, especially when dealing with untrusted data on a web application because not properly implementing safeguards for different kinds of attacks and exploits can lead to loss of money, server downtime and stolen information.  Software security adds immense value as a company needs its sensitive information protected, the confidence of its customers that their data is safe, and protection from exploits that can lead to money lost, either by direct theft or denial of service. 

•	What about the process of working through the vulnerability assessment did you find challenging or helpful?

I found identifying the security areas to inspect based on the initial prompt challenging at first.  I inspected a few extra areas that turned out to be irrelevant for Artemis’s scenario, but I felt that was better than missing critical areas to inspect.                                                                                                                                                                                                                                                                                                                                                                                                                                        
•	How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?

I approached the need to increase layers of security by focusing on one relevant area at a time. I found the vulnerability assessment process flow a great piece of information to find these relevant areas and would use it again in the future, along with my notes of our textbook: Iron-Clad Java: Building Secure Web Applications.  The National Vulnerability Database (NVD ) was also a great resource as it provided a multitude of mitigation techniques for known vulnerabilities. 


•	How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?

I ensured the code was functional by simply testing it until it was an acceptable form. I ensured it was secure by following security best practices for writing code that implemented the desired functionality. If what I was writing required a new dependency to the project, I would run a dependency check report and examine any newly introduced vulnerabilities . 

•	What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?

I found the java key tool very helpful in creating SSL certificates with their keys and keystores. I would use this in future java web projects when setting up SSL for HTTPS. I also found the Maven dependency checker to be very informative, providing vulnerability reports from the NVD that can be tuned to exclude false positives. I also employed a checksum through a method I learned in java that uses the messageDigest class which I would reuse. 

•	Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?

From this project, the thing  I would showcase to a future employer would be my breakdown of manual code inspections with the solutions I provided to mitigate the weak points in the code. 
