# CS-305-Module-Eight-Journal-
1. Briefly summarize your client, Artemis Financial, and its software requirements.

Artemis Financial is a consulting company that develops individualized financial plans for its customers, including savings, retirement, investments, and insurance. The company wanted to modernize its operations while improving the security of its web application. Specifically, Artemis Financial wanted to protect its clients' personal and financial information by implementing secure communication methods and adding a checksum to verify data integrity during transfers.

2. What did you do well when you found your client's software security vulnerabilities? Why is it important to code securely?

I think what I did well was learning how to perform vulnerability assessments using Maven and OWASP Dependency-Check. I was able to identify vulnerabilities, determine which libraries they belonged to, and update the dependencies in the pom.xml file to address them. I also learned how to use an updated version of Dependency-Check to identify known vulnerabilities more effectively. It is important to code securely because vulnerabilities can expose applications to unauthorized access, malicious attacks, and data leaks. Keeping software secure helps protect sensitive information, maintain customer trust, and reduce risks to the company.

3. Which part of the vulnerability assessment was challenging or helpful to you?

The most challenging part was identifying the multiple libraries associated with the vulnerabilities and determining which dependencies needed to be updated. Some libraries were connected to other dependencies, which made the process more complicated. However, this was also one of the most helpful parts of the project because I learned how to investigate vulnerabilities, update dependencies, and run additional scans to verify whether the changes addressed the issues.

4. How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?

I increased the layers of security by implementing SHA-256 hashing to generate a checksum, configuring HTTPS to protect communication, and updating vulnerable dependencies. I also generated a self-signed certificate using Java Keytool and configured the application to use it during local testing. In future projects, I would use OWASP Dependency-Check to identify known vulnerabilities, review the affected libraries and their versions, and determine which updates or security measures would best address the risks.

5. How did you make certain the code and software application were functional and secure?

After refactoring the code, I used Maven to rebuild the application and performed another OWASP Dependency-Check scan to identify any remaining known vulnerabilities. The initial scan identified 14 vulnerable dependencies and 254 vulnerability findings. After updating the libraries, the final scan reported zero vulnerable dependencies and zero vulnerability findings. I also tested the application in Eclipse and confirmed that the HTTPS endpoint worked and generated the expected SHA-256 checksum. Although these results do not guarantee that the application is completely secure, they show that the changes reduced the known security risks detected during testing.

6. What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?

The main tools I used were Eclipse, Maven, OWASP Dependency-Check, Java Keytool, and Java's MessageDigest class. I also learned how to configure HTTPS, manage dependencies through pom.xml, and use SHA-256 hashing. These tools and practices will be helpful in future projects because they allow me to identify vulnerabilities, implement security measures, and verify that an application continues to function correctly after changes.

7. What might you show future employers from this assignment?

I would show future employers my Artemis Financial Practices for Secure Software Report because it demonstrates my ability to identify and address software security vulnerabilities. One of my biggest accomplishments was reducing 254 vulnerability findings to zero detected findings by identifying affected libraries and updating dependencies. I would also highlight my experience implementing SHA-256 hashing, configuring HTTPS, and performing functional and security testing. This project helped me develop skills in secure coding, vulnerability assessment, troubleshooting, and dependency management that I can apply to future software development projects.
