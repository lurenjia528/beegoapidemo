beego api demo

```mysql
 CREATE TABLE `student` ( 
       `Id` int(11) NOT NULL, 
       `Name` varchar(10), 
       `Birthdate` date , 
       `Gender` tinyint(1) , 
       `Score` int(11), 
       PRIMARY KEY (`Id`) 
     );
```

`bee api beegoapidemo -tables="student" -driver=mysql -conn="root:123123@tcp(127.0.0.1:3306)/test"`

项目目录下运行 
```bash
bee run  -gendoc=true -downdoc=true
```
会在项目目录下产生swagger目录,

访问
`http://127.0.0.1:8080/swagger/`
