# EEIT45 SpringMVC 作業 CRUD


### 說明

-  1.請先建立好 SQL 檔案 
-  2.請先建立好 Server content.xml

#### 目錄結構

## Server(Tomcat) Content.xml
```
 <Resource 
     name="connectSqlServerJdbc/SystemService"
	  type="javax.sql.DataSource" 
	  auth="Container" 
	  username="sa"
	  password="sa123456"
	  driverClassName="com.microsoft.sqlserver.jdbc.SQLServerDriver"
	  url="jdbc:sqlserver://localhost:1433;databaseName=firstGroup" />
```


## T-SQL 
```
use firstGroup; 

drop table if exists reserve;

create table reserve(
id int NOT NULL IDENTITY(1,1),  
reserveName nvarchar(50) not null,
reserveDate nvarchar(50) not null,
reserveRestuarant nvarchar(50) not null
);

```
