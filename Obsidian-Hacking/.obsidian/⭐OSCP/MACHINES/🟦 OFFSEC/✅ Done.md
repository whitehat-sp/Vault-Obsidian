```dataview
table machine,Fecha-Hack
from "OSCP/MACHINES/HTB"
where Plataforma = "HTB" and status = "Done"
sort owned_date desc
limit 1
```

