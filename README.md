# CS305
CS 305 Repository
Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?
Artemis Financial is a financial consulting company that develops individualized financial plans for savings, retirement, investments, and insurance for a global clientele. The company wanted to modernize its application, a RESTful API, and address significant software security vulnerabilities to protect its highly sensitive customer financial data from external threats.

What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?
I conducted a thorough, multi-faceted vulnerability assessment that combined a detailed manual code review with static testing using the OWASP Dependency-Check tool. This approach allowed me to identify everything from high-level architectural issues and SQL injection vulnerabilities in the custom code to known vulnerabilities in third-party libraries like Bouncy Castle. Coding securely is crucial because it is the primary defense against data breaches, financial fraud, and loss of customer trust. For a company like Artemis Financial, strong software security directly protects its reputation, ensures legal and regulatory compliance, and safeguards its financial stability.

Which part of the vulnerability assessment was challenging or helpful to you?
The manual code review was particularly challenging as it required meticulous inspection to find logical flaws and insecure coding practices that automated tools might miss, such as hard-coded credentials, poor encapsulation, and generic exception handling. However, this process was also extremely helpful in developing a deep understanding of how vulnerabilities are introduced at the code level.

How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
I increased security layers by refactoring the code to mitigate specific vulnerabilities, like using parameterized queries for SQL injection, and by adding new security features. This included implementing SHA-256 for secure data verification and configuring the application to use HTTPS for all client-server communications, thereby encrypting data in transit. In the future, I would use a combination of manual code review, static analysis tools like OWASP Dependency-Check, and dynamic analysis tools to comprehensively assess vulnerabilities, prioritizing mitigation based on severity and potential business impact.

How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
After refactoring, I performed functional testing to ensure the application operated correctly with the new security features. I then ran the OWASP Dependency-Check tool again to scan for any new vulnerabilities in the dependencies and conducted a secondary manual code review of the refactored code to verify that the fixes were properly implemented and did not introduce new security issues.

What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
The OWASP Dependency-Check tool was invaluable for automating the detection of vulnerable libraries. Key coding practices included adopting the principle of least privilege for data access, using parameterized queries to prevent injection attacks, and following industry standards like implementing strong cryptographic hashing (SHA-256) and enforcing HTTPS.

Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
From this assignment, I would showcase the completed Vulnerability Assessment Report to demonstrate my ability to systematically identify and analyze security vulnerabilities in a codebase. I would also present the Practices for Secure Software Report to highlight my practical skills in refactoring code to mitigate those vulnerabilities and implement robust security controls like checksum verification and secure HTTPS communication.
