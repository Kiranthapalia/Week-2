# Week-2

## 1. Read and Summarize

### OWASP: OWASP 10 2021.
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
### Darknet Diaries.
  - Episode 6: The Beirut bank job was chosen for the Darknet Diaries. In essence, it tells the story of a man named Jason who unintentionally robbed the         wrong bank in Beirut. little details about him Jason began his career in law enforcement but has spent the most of the previous twenty years in infosec.
    He has put in a lot of effort protecting the network, but he has also conducted a lot of penetration testing.
  - One of his favourite activities is what he calls Security Awareness Engagement, which involves teaching people about the danger that truly exists rather     than engaging red teams or performing pin tests.Companies hire him to evaluate a location's physical security. Even National Geographic videotaped him       doing some of the things he talks about in an episode.
  - He was given 3 chances to actually compromise the network in 3 different banks. Typically, he uses a pwn plug, a USB rubber ducky, possibly a Proxmark3       tool, a few Dropboxes, or other malicious items to demonstrate to them the harm he is capable of causing to their networks.
  - As a result, what he essentially does is fabricate an incident or a distraction to lead the bank employees to believe that he is acquainted with those in     positions of authority by making it appear as though he had just left the manager's or supervisor's room. After that, he just poses as an IT                 professional, plugs in his rubber ducky, and uses their mouse while in control of it.
  - He basically did that to gain access to all the other banks, but when a bank employee questioned him for his ID and he displayed his phony ID and bogus       email, he got into difficulty at the last branch he was supposed to attack. He was then informed that in order to proceed, he must visit the supervisor.
  - He believed there were only two possibilities: either they would believe him or they would require more evidence. He also believed he had the option of       leaving since he had already accomplished his goal, but there was a third possibility: compromising the wrong bank and being discovered.
  - Because he didn't know Arabic, it was now impossible for them to grasp that he had actually been hired to rob a bank but had unintentionally robbed the       incorrect one.  Only after spending many hours being questioned and meeting with the bank's security team and convincing from the man who had hired him       to compromise was he permitted to leave, and even then he didn't feel safe until he got back to Paris.
  
    #### Lesson Learned 
    - It is acceptable for them to be suspicious when someone walks in and to call someone to confirm the presence of someone new.
    - Robbers not only have weapons and ski masks, but also suits and USB drives.
    - Regardless of whether you expected it or not, be wary of certain e-mails that appear to be from - and include a link to.
    #### How could it have been avoided?
    - By verifying individuals who do not appear to be familiar.
    - By not allowing anyone to accompany you into the building with your ID and badge.
    - being firm but not rude, informing them of the security policy while verifying.
    - By not allowing someone to use the company's computer without permission.
### CVE
 - Red Hat has recently been designated as a CVE Program Root for open-source software for any projects or existing CNAs that prefer Red Hat as their Root.
 - A Root in the CVE Program is an organization authorized within the CVE Program that is responsible for the recruitment, training, and governance of one or    more CNAs within a specific scope.
 - CVE Program Partner Since 2002 Red Hat partnered with the CVE Program as a CNA in 2002.
  #### Why it matters.
  
