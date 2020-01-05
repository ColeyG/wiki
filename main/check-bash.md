# Check Before Process in Bash

```bash
if [[ $(ps -a | grep anydesk) ]]; then
  echo "Anydesk instance found";
else
  echo "No Anydesk Instance found";
  anydesk;
fi
```
