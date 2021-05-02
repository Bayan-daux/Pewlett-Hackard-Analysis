#**Pewlett Hackard Analysis**

##**Overview**

This project is a hypothetical scenario in which an HR analyst at company called *Pewlett Hackard* is tasked to preform employee research. PH is a large company, boasting several thousand employees and it has been around for a long time. As baby boomers begin to retire at a rapid rate, PH is looking towards the future in two ways. First, it’s offering a retirement packages for those who meet certain criteria. Second, it is starting to think about which position will need to be filled on the near future. The number of upcoming retirements will leave thousands of job openings. PH is looking ahead and starting to prepare for these many vacancies. Therefore, the HR Analyst will perform the tasked research and help the company leadership in answering the following questions: 

1. Who will be retiring in the next few years, and, of those employees, 
   who is eligible for a retirement package?
1. How many positions will PH need to fill?

The analysis will help future proof PH by generating a list of all employees eligible for retirement package. As PH has been mainly using Excel and VBA to work with their employee data, its data is only available in a form of CSV files. However, currently they decided to update their methods and build a database to house all their data using *SQL*.  

- **The process and outcomes for this project**

To build the database *PostgreSQL* and *pgAdmin* were used. Starting by modeling the data by creating entity relationship diagrams (ERDs) using *QuickDBD*. Then importing company’s available data (*six CVS files: departments.csv, employees.csv, dept\_manager.csv, salaries.csv, dept\_emp.csv, titles.csv*) into the database, troubleshoot common errors. Them followed by creating queries that use the employees’ data to answer the questions stated above. (output files*: retirement\_info.csv, current\_emp.csv,* *current\_emp\_by\_dept.csv)*

After achieving the initial required task and knowing that around **90,398** employees leaving PH soon from seven different department, with **41,380** of them eligible for a retirement package (*figure 01*), PH has requested three additional lists that are more specific to dive deeper into the data. 

(current_emp_by_dept.png)

*figure 01*

1. **Employee Information:** A list of employees containing their unique employee number, their last name, first name, gender, and salary (output file*: retirement\_info.csv*) 
1. **Management:** A list of managers for each department, including the department number, name, and the manager's employee number, last name, first name, and the starting and ending employment dates (output file*: manager\_info.csv*)
1. **Department Retirees:** An updated current\_emp list that includes everything it currently has, but also the employee's departments. (output file*: dept\_info.csv*)

Beside these lists answering the company questions regarding their employee retirement, each list has also raised other questions such as, what’s going on with the salaries? Why are there only five active managers for nine departments? And so on. To answer such questions, some tailored lists were created (output files: *sales\_info.csv, sales\_dev\_info.csv*)

After achieving the requested analysis. A second follow up analysis was requested. The aim is to determine the number of retiring employees per title and identify employees who are eligible to participate in a mentorship program. 

##**Results**

- Retirement-Eligible Employees with Titles (*Figure 02)* (Output File: *retirement\_titles.csv*)

![Graphical user interface

Description automatically generated](Aspose.Words.46bc5e4b-9120-4958-a557-51e181d0c9d3.002.png)

*Figure 02*

- Retirement-Eligible Employees with Titles (*Figure 03)* (Output File: *.csv*) 

(Aspose.Words.46bc5e4b-9120-4958-a557-51e181d0c9d3.003.png)

*Figure 03*

- Number of Retirement-Eligible Employees by Most Recent Title (*Figure 04)* (Output File: retiring\_titles.csv)

![Graphical user interface, application, table

Description automatically generated](Aspose.Words.46bc5e4b-9120-4958-a557-51e181d0c9d3.004.png)

*Figure 04*

- Employees Eligible for Mentorship Program (*Figure 05)* (Output File: mentorship\_eligibility.csv)

![Graphical user interface, table

Description automatically generated](Aspose.Words.46bc5e4b-9120-4958-a557-51e181d0c9d3.005.png)

*Figure 05*

##**Summary**

Based on the results form all analysis here is some insight into the upcoming *silver tsunami,* PH needs to be aware of. As mentioned above, there are a total of **90,398** employees leaving, **41,380** of them in the very near future working on all seven of the company departments, who are also eligible for a retirement package. All these positions will need to be filled soon. 

Regarding the mentorship program eligibility, more queries were done to understand the results better. The results indicated there are only **1,549** retirement ready employees who are eligible to mentor younger ones. However, more importantly, there are zero of these employees in a manager position, which indicating a huge problem that needs immediate address by PH, the ability to train the next generation of employees into future mangers (figure 06).

![Graphical user interface, table

Description automatically generated](Aspose.Words.46bc5e4b-9120-4958-a557-51e181d0c9d3.006.png)*

*Figure 06*
