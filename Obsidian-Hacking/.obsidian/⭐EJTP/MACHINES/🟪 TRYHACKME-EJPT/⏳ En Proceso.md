```dataview
table machine, Dificultad, Fecha-Run
from "EJPT/MACHINES/TRYHACKME"
where Plataforma = "HTB" and status = "En Proceso"
sort owned_date desc
limit 1
```

