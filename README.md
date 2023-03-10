# Week-2

## X. Read and Summarize

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
  - Because he didn't know Arabic, it was now impossible for them to grasp that he had actually been hired to rob a bank but had unintentionally robbed the       incorrect one.?? Only after spending many hours being questioned and meeting with the bank's security team and convincing from the man who had hired him       to compromise was he permitted to leave, and even then he didn't feel safe until he got back to Paris.
  
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
    - It is a pleasure and a proud moment for Red Hat to contribute to sharing our CVE story of how and why we became a Root, as well as how we contribute to       the CVE Program's coverage of open-source software.
    - They work hard to protect customer, contributor, and partner communities from digital security threats.
    - They believe that following open-source principles is the best way forward.
    - Red Hat Product Security has consistently shown a proactive approach to identifying issues in the products we ship.
## A. SQL
  ### 0 SELECT basics
  ![SQL0](https://user-images.githubusercontent.com/102954934/215616798-e7d044a8-0c8f-4bf1-89da-320d9d3ea6a7.jpeg)

    As a former Database Management System this was a piece of cake for me. I just used tha basic Where statement all 3 of those tasks.
  ### 2 SELECT from World
  ![SQL 2](https://user-images.githubusercontent.com/102954934/215617195-d54609cf-3f97-47aa-bfba-f85f71a1862e.jpeg)
  This was fairly easy aswell. We were supposed to do just 5 tasks but I did all of them because it was easy. 
  - The first 4 tasks were similar to the one we did earlier using th basic `WHERE` statement. 
  - No 5 was similar but incase of using where name = 'germany'OR where name = 'France' etc we just used where name in ('Germany', 'France') to save time. 
  - NO 6 we had to find the countried that had the word united in it so we used %united%. 
  - No 7 This was same as before using the `WHERE` statment following with conditions.
  - N0 8 The XOR (exclusive or) did not really work for me so i used the where statement where it met just one condition.
  - NO 9 We just had to use the `Round` statement and show the population in millions by dividing it by 1000000 and GDP in billions by dividing it by             1000000000.
  - NO 10 It was also pretty much the same except we had to round the value to the nearest 1000$ so i just used the round statement as shown in the fig.
  - NO 11 Here LENGTH did not work so i had to use LEN , even thought the ans was correct, it did not show anything.
  - NO 12 This was about matching the firstt letter of name and capital so I used LEFT(name,1)=LEFT(capital,1) and <>(not equals to).
  - NO 13 This was a bit tricky not because it was difficult but because it was not working in the website but it was working on my own sql. I juse used         WHERE like '%a%' and then or for rest of the vowel with similar statments and Not like '% %' for the space.

## B. Injected. Solve WebGoat:
  <img width="352" alt="webgoat1" src="https://user-images.githubusercontent.com/102954934/215622422-70b14d37-120f-43d0-97b9-692bb78990e7.png">
  
  - `SELECT department FROM Employees WHERE first_name='Bob'` Here we can also add AND last_name='Franco' incase there are two Bob.
  
  <img width="380" alt="wg2" src="https://user-images.githubusercontent.com/102954934/215623151-87ee4ec9-449e-45b9-b1a8-9079432ffbc8.png">
  
  - `UPDATE Employees SET department='Sales' WHERE first_name='Tobi' AND last_name='Barnett';`
  
  <img width="361" alt="wg3" src="https://user-images.githubusercontent.com/102954934/215623331-7815ec2a-d8f3-4720-80a3-1beafb1fc5e4.png">
  
  - `ALTER TABLE Employees ADD phone VARCHAR(20);`
  
  <img width="359" alt="wg4" src="https://user-images.githubusercontent.com/102954934/215623537-233506d1-31fe-440e-af95-1c377a89dbbf.png">
  
  - `GRANT ALTER TABLE TO UnauthorizedUser;`
  
  <img width="358" alt="wg5" src="https://user-images.githubusercontent.com/102954934/215623847-52751493-4f64-48e1-9001-0b9b8053f3f3.png">
  
  First SQL injection happens because the input is put straight into the query:
 `SELECT * FROM user_data WHERE first_name='John' AND last_name='' OR '1'='1';`
 
 <img width="401" alt="wg6" src="https://user-images.githubusercontent.com/102954934/215627496-4b7ceb5d-63ff-458a-9cd5-cbf8d1f53839.png">
 
 `' OR '1'='1` I tried this many time trying to figure out what to use.
 
 <img width="414" alt="wg7" src="https://user-images.githubusercontent.com/102954934/215627692-6b6abf1b-45ca-4e30-9643-5396da978a30.png">
 
 `(Login_Count) 1 and (User_Id)'123' OR '1'='1' ` This one literally took me 10-15 to figure out.
 
 <img width="375" alt="wg8" src="https://user-images.githubusercontent.com/102954934/215627941-376a985e-5ca2-4a19-ae9a-a6fe16917c16.png">
 
 Inputing in the  fields (Employee Name and Authentication TAN)
 (name) Tan' OR '1'='1  and (Authentication TAN) 3NJ92A' OR '1'='1 . Did a lot of googling to figure this out.
 
 <img width="755" alt="w9" src="https://user-images.githubusercontent.com/102954934/215629146-1c148922-8596-4035-ba84-71f1d9a1a99d.png">
 
 `3SL99A';UPDATE Employees SET salary=100000 WHERE last_name='Smith' AND auth_tan='3SL99A';--`
 Found another solution : asd'; UPDATE employees SET salary = '999999' where userid='37648'--
 This one was just raising the salary so updating the table worked.
 
 <img width="733" alt="wg10" src="https://user-images.githubusercontent.com/102954934/215629431-2533240d-b552-4aa0-b036-31d4e8705c15.png">
 
 `'; DROP TABLE access_log;--`
 Just had to drop table.

## Sources
  - https://terokarvinen.com/2021/data-security-2022p3-ict4tf022-3008/#h2
  - https://owasp.org/Top10/A05_2021-Security_Misconfiguration/
  - https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/
  - https://owasp.org/Top10/A03_2021-Injection/
  - https://darknetdiaries.com/episode/6/
  - https://www.cve.org/Media/News/item/blog/2023/01/10/Why-Red-Hat-Became-Root
  - https://www.arbexam.blog/webgoat-sql-injection-intro/
