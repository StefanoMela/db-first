# DB-FIRST

### Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario.

COLONNA | TIPO | ATTRIBUTI
-- | -- | --
id | bigint | PRIMARY KEY, A_I
brand | varchar(20) | NOT NULL
model | varchar(50) | NOT NULL
tot_km | mediumint | UNSIGNED, NOT NULL
condition | tinyint | UNSIGNED, NOT NULL, DEFAULT(6)
color | varchar (15) | NULL
engine_type | char(1) | NOT NULL
engine_power | smallint | NULL
traction | char(3) | NULL
owner_number | tinyint | NULL, DEFAULT (1) 
price | smallint | UNSIGNED, NOT NULL
plate_number | char(7) | UNIQUE, NOT NULL


### Explanation

## condition 
- integer rating from 1 to 10: 1 worst condition ever - 10 best condition possible

## engine_type
- refers to the first letter of the engine type: 
 - (E)lectric
 - (M)ild
 - (H)ybrid
 - (D)iesel
 - (O)il
 - (G)pl

## traction 
- refers to the frist letter of traction type: 
- AWD - all-wheel-drive
- FWD - forward-wheel-drive
- RWD - rear-wheel-drive
- 4WD - four-wheel-drive



