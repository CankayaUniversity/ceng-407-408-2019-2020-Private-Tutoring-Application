# ceng-407-408-2019-2020-Private-Tutoring-Application
Private Tutoring Application

# Team Members

* Hande Aydın - 201511410
* Eyüp Can Turğut - 201411062
* Damla Yıldırım - 201411068
* Serhat Cenkayoğlu - 201511301

# Compilation / Installation Guide (for Windows)

Before starting, make sure that you have installed [Visual Studio 2019](https://visualstudio.microsoft.com/tr/vs/) (it supposed to include _ASP.NET and web development_) and [PostgreSQL](https://www.postgresql.org/) on your computer.
<br />

### Step 1
Open pgAdmin application. (pgAdmin is the most popular and Open Source administration and development platform for PostgreSQL.) To find the application easily, click search button on taskbar and type "pgadmin".

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80656472-f7c11400-8a89-11ea-92ce-430c4d081b6a.png"></p>

### Step 2
Enter your password. Then click on _Servers_' arrow at its left.

**Note:** After clicking arrow, it is possible that it may ask you to enter your password again.

### Step 3
Right click on _Databases_. Then select _Create > Database..._.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658268-60aa8b00-8a8e-11ea-97f1-28300f9153a5.PNG"></p>

### Step 4
Enter a Database name and save it. It could be anything that you want.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658301-7750e200-8a8e-11ea-899a-95a045069916.PNG"></p>

### Step 5
Click on database at left that you have just created. It will connect the database and notify you that it is connected.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658356-92bbed00-8a8e-11ea-8ebc-70b6054c99ac.PNG"></p>
<p align="center"><i>Nodification</i></p>

### Step 6
Download the project from [Releases](https://github.com/CankayaUniversity/ceng-407-408-2019-2020-Private-Tutoring-Application/releases). Extract it and open _PrivateTutoringApplication.sln_ file.

### Step 7
From Solution Explorer, click _appsettings.json_ file.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658392-ab2c0780-8a8e-11ea-8d4c-113572dbebcd.PNG"></p>

### Step 8
Change _Password_ and _Database_ fields as shown below and save it.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658451-d151a780-8a8e-11ea-94ab-9c80c7621397.PNG"></p>

### Step 9
From Solution Explorer again, click _PrivateTutoringApplication.Model > Infrastructure > DatabaseContext.cs_ file.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658482-e1698700-8a8e-11ea-956a-d375f253bedd.PNG"></p>

### Step 10
Change _Password_ and _Database_ fields like previous step and save it.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658509-f3e3c080-8a8e-11ea-8475-3684bffe045c.PNG"></p>

### Step 11
Click on _Package Manager Console_ at bottom.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658535-078f2700-8a8f-11ea-8d59-26a35b2eb95e.PNG"></p>

### Step 12
Set _Default Project_ field as _PrivateTutoringApplication.Model_.

<p align="center"><img src="https://user-images.githubusercontent.com/48491124/80658549-1544ac80-8a8f-11ea-9ffc-0e4a7c62c0d5.PNG"></p>

### Step 13
Type the code below to console and press enter.
```
Add-migration anyname
```
**Note:** Instead of `anyname`, you could type anything you want, it doesn't matter. This will compare and find difference between datababase and model code.

When it's built succeeded, the console will notify you as below.

<p><img src="https://user-images.githubusercontent.com/48491124/80658653-5e94fc00-8a8f-11ea-895a-c5fa15336a0b.PNG"></p>

### Step 14
Type the code below and enter.
```
Update-database
```

If succeed, the console will notify you as below.

<p><img src="https://user-images.githubusercontent.com/48491124/80658685-77051680-8a8f-11ea-9e2c-999e653b9d2a.PNG"></p>

### Step 15
That's it! You can run the application by clicking _IIS Express_ button at top.
