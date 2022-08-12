# Pierre's Sweet and Savory Treats

#### By _**Frank Timmons**_  

#### _A savory treat website that allows you to keep track of all your flavors and treats!._  

---


## Technologies Used

* _C#_
* _.NET_
* _HTML_
* _CSS_
* _SQL Workbench_
* _Entity Framework_
* _MVC_
* _Identity_

---
## Description

_This is an MVC application that was built using C#. It lets you create and log into an account. While you're logged in, it allows you to add flavors and treats to a shop, and associate them with eachother in a many to many relationship. It allows you to add, edit, and delete them as you please. If you're not logged in, you can only view the list of all flavors/treats/ and their details pages._

---
## Setup and Installation Requirements
**This Setup assumes you have GitBash and MySQL Workbench pre-installed.   
If needed, please navigate to these links:  
https://git-scm.com/download/  
Download Git and follow the setup wizard.  
https://dev.mysql.com/downloads/workbench/  
Download MySQL Workbench, follow the setup wizard & create a localhost server on port 3306**


*Note: Keep track of your username and password, this will be used in the connection link under,*  
"**SQL Workbench Configuration**" > "2. Insert the following code:"

<details>
<summary><strong>Initial Setup</strong></summary>
<ol>
<li>Copy the git repository url: https://github.com/FrankTimmons/PierresTreats.Solution
<li>Open a terminal and navigate to your Desktop with <strong>cd</strong> command
<li>Run,   
<strong>$ git clone https://github.com/FrankTimmons/PierresTreats.Solution</strong>
<li>In the terminal, navigate into the root directory of the cloned project folder "PierresTreats.Solution".
<li>Navigate to the projects root directory, "PierresTreats".
<li>Move onto "SQL Workbench Configuration" instructions below to build the necessary database.
<br>
</details>

<details>
<summary><strong>SQL Workbench Configuration</strong></summary>
<ol>
<li>Create an appsetting.json file in the "PierresTreats" directory  
   <pre>PierresTreats.Solution
   └── PierresTreats
    └── appsetting.json</pre>
<li> Insert the following code: <br>

<pre>{
  "ConnectionStrings": {
    "DefaultConnection": "Server=localhost;Port=3306;database=frank_timmons;uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}</pre>
<small>*Note: you must include your password in the code block section labeled "YOUR-PASSWORD-HERE".</small><br>
<small>**Note: you must include your username in the code block section labeled "YOUR-USERNAME-HERE".</small><br>
<small>***Note: if you plan to push this cloned project to a public-facing repository, remember to add the appsettings.json file to your .gitignore before doing so.</small>

<li>In root directory of project folder "PierresTreats", run  
<strong>$ dotnet ef database update</strong></li>


<ol> 
  <li>Open SQL Workbench.
  <li>Navigate to "frank_timmons" schema.
  <li>Click the drop down, select "Tables" drop down.
  <li>Verify the tables, you should see <strong>treats</strong>, <strong>flavors</strong>, and <strong>flavortreat</strong></li>
</ol>
  
</details>

<details>
<summary><strong>To Run</strong></summary>
Navigate to:  
   <pre>PierresTreats.Solution
   └── <strong>PierresTreats</strong></pre>

Run ```$ dotnet restore``` in the terminal.<br>
Run ```$ dotnet run``` in the terminal.<br>
</details>

<br>

---

Big Thanks to Garrett Hays @ https://github.com/GarrettHays, and Grace Kostanich @ https://github.com/User8240 for amazing README formatting and instructions!

## Known Bugs

* _No known bugs_

## License

[MIT](/LICENSE)

Copyright (c) 2022 Frank Timmons