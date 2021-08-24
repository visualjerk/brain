# Bashscripts

## Functions

Using functions in bash:

```bash
greet ()
{
	local greeting='Hello'
	echo "$greeting $1"
}

greet "Pete" # Hello Pete
```