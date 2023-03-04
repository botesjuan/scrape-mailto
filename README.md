# scrape-mailto
Find email addressed in HTML source, by searching for string ```mailto:```.  

Then use bash script to run through multiple target URL web sites.

```bash
#!/bin/bash

while read line; do
  python scrape-mailto-v2.py "$line" >> "output_results.txt"
done < web-urls-list.txt
```  

View the content of the results ```cat output_results.txt```  
