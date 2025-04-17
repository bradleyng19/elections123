---
title: General Election Manpower Requirements
---

<Details title= General Election Manpower Requirements>

  This page can be found in your project at `/pages/index.md`. Make a change to the markdown file and save it to see the change take effect in your browser.
</Details>


# CENTRAL 1 ZONE 1

```sql Central1Z1
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date, 
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z1%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central1Z1
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z1%'
GROUP BY zone
```

<DataTable data={total_Central1Z1}/>

<DataTable data={Central1Z1}/>

# CENTRAL 1 ZONE 2

```sql Central1Z2
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date,
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z2%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central1Z2
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z2%'
GROUP BY zone
```

<DataTable data={total_Central1Z2}/>

<DataTable data={Central1Z2}/>

# CENTRAL 1 ZONE 3

```sql Central1Z3
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date,
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z3%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central1Z3
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central1%'
AND zone ILIKE 'z3%'
GROUP BY zone
```

<DataTable data={total_Central1Z3}/>

<DataTable data={Central1Z3}/>

# CENTRAL 2 ZONE 4

```sql Central2Z4
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date,
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central2%'
AND zone ILIKE 'z4%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central2Z4
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central2%'
AND zone ILIKE 'z4%'
GROUP BY zone
```

<DataTable data={total_Central2Z4}/>

<DataTable data={Central2Z4}/>

# CENTRAL 2 ZONE 5

```sql Central2Z5
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date,
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central2'
AND zone ILIKE 'z5%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central2Z5
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central2%'
AND zone ILIKE 'z5%'
GROUP BY zone
```

<DataTable data={total_Central2Z5}/>

<DataTable data={Central2Z5}/>

# CENTRAL 2 ZONE 6

```sql Central2Z6
Select 
Loc_type,
zone,
STRFTIME(
    STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y'),
    '%d %b') AS parsed_date,
Start_shift,
end_shift,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
from ge_location
WHERE sector ILIKE 'central2%'
AND zone ILIKE 'z6%'
GROUP BY DATE,loc_type, zone, start_shift, end_shift
ORDER BY zone, STRPTIME(REPLACE(REPLACE(LOWER(date), '_', '-'), ' ', '-') || '-2000', '%d-%b-%Y')
```

```sql total_Central2Z6
SELECT 
zone,
SUM(Saro_IC) AS Total_num_SaroIC,
SUM(Log_ic) AS Total_num_LogIC,
SUM(crew) AS Total_num_Crew
FROM ge_location
WHERE sector ILIKE 'central2%'
AND zone ILIKE 'z6%'
GROUP BY zone
```

<DataTable data={total_Central2Z6}/>

<DataTable data={Central2Z6}/>
