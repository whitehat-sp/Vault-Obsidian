```dataview
table machine,Fecha-Hack
from "EJPT/MACHINES/TRYHACKME"
where Plataforma = "HTB" and status = "Done"
sort owned_date desc
limit 1
```

