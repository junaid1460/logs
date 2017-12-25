### converting string into array based on delimitter in bash

```shell
string="1 2 4 4"
IFS=' ' # space as delimitter
read -r -a array << "$string" 

```
