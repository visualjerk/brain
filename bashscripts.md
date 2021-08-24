# Bashscripts

## Functions

```bash
greet ()
{
	local greeting='Hello'
	echo "$greeting $1"
}

greet "Pete" # Hello Pete
```

## Replace String In File

Replace `foo` with `#foo` globally and create a backup.

```bash
sed -i.bakup "s/foo/#&/g" "./myfile.txt"
```

Make use of extended regex (needed for `+` and grouping) with `-E`

```bash
sed -i.bakup -E "s/foo.+/#&/g" "./myfile.txt"
```