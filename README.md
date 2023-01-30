# Week-2

## 1. Read and Summarize

### OWASP: OWASP 10 2021
  #### A05:2021-Security Misconfiguration.
    - The number of apps analyzed increased from 6 in the previous edition to 90%, with an average incidence rate of 4% and more than 208k occurrences of a           Common Weakness Enumeration CWE in this risk area.
    - It's not unexpected to see this category advance given the increasing changes toward highly customizable software.
    - Two notable CWEs are CWE-611 Improper Restriction of XML External Entity Reference and CWE-16 Configuration. 
    - If the program lacks adequate security hardening across any portion of the application stack or has wrongly configured permissions on cloud services, the       application may be susceptible. 
    - Unneeded ports, services, pages, accounts, or privileges, for example, are enabled or installed. The default accounts are still active, and their               passwords are unaltered.
  #### A06:2021-Vulnerable and Outdated Components.
    - Although it came in at number two in the Top 10 Community Survey, it had enough data to crack the Top 10 via data.
    - Given that there is a recognized problem with testing and assessing risk for vulnerable components, which is the sole category without any Common               Vulnerabilities and Exposures CVEs mapped to the included CWEs, a default exploitsimpact weight of 5.0 is applied.
    - The two CWEs from the 2013 and 2017 Top 10 as well as CWE-1104 Use of Unmaintained Third-Party Components are noteworthy CWEs.
    - You are probably vulnerable: if you don't frequently scan for vulnerabilities and if software developers fail to check if upgraded, patched, or updated         libraries are compatible.
    - To stop something like that from happening Obtain components only from reputable suppliers using secure channels. Keep an eye out for libraries and             components that lack maintenance or don't produce security updates for previous iterations.
  #### A03:2021-Injection.
    - The third position for injection is a downward slide. A maximum incidence rate of 19%, an average incidence rate of 3%, and 274k occurrences were tested         for injection in 94 of the applications.
    - Important Common Weakness Lists CWE-79 Cross-site Scripting, CWE-89 SQL Injection, and CWE-73 External Control of File Name or Path are among the CWEs           that are present.
    - When user-provided data is not verified, filtered, or sanitized by the program, the application is open to attack.
    - To avoid this Use LIMIT and other SQL controls within queries to prevent bulk record exposure in the event of SQL injection. Also, use affirmative server-       side input validation.
    - Attack scenario examples The following susceptible SQL call is built by an application using unreliable data:
      `String query = "SELECT \* FROM accounts WHERE custID='" + request.getParameter("id") + "'";`
    
