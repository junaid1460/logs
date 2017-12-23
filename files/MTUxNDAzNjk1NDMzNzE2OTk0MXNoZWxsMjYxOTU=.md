## script for renaming files in a directory recursively

```shell
dir="bm"
IFS=$'\n'
for i in `ls $dir`;do
        newname=`cut -d'?' -f1 <<< $i`
        echo $newname
        mv "$dir/$i" "$dir/$newname"
done
```

