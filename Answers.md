**1.**   
Affiliate   
Bank   
Client   
Employee   
Parent   
Prospect    
ServiceBureau    
System    
TaxAgency    
Vendor    

```
select Distinct EntityType
from Stage.dbo.e_entity
```


**2.**   
CougarLand   

```
select EntityOwner
from Stage.dbo.e_entity
where city = 'Alex'
```


**3.**   
13/14   

```
select LegalName
from Stage.dbo.e_entity
where ContactMethod IS NULL
```

**4.**  
Regional Income   

```
select LegalName
from Stage.dbo.e_entity
where ContactMethod = ''
```

**5.**   
1828   

```
select entity
from Stage.dbo.e_entity
where StartDate > '2020-01-01'
```

**6.**  


```
select City, State
from Stage.dbo.e_entity
where Zip Between '77478' AND '77483'
```

**7.**  
S-Corp

```
select IncorporationType
from Stage.dbo.e_entity
where Country = 'CAN' AND EntityOwner = 'TAGSB'
```

**8.**  
Tricomcorp   
Empower   

```
select FilterClient
from Stage.dbo.e_entity
where LegalName = 'Wells Fargo Bank' AND Address1 IS NULL
```

**9.**  
107   

```
select *
from Stage.dbo.e_entity
where (StartDate BETWEEN '2015-07-01' AND '2015-07-01') or UserType = 'CPA'
```

**10.**   
danny

```
select *
from Stage.dbo.e_entity
where Country <> 'USA' AND Shift = 'Day'
```


