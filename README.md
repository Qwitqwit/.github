# Qwitqwit

A collction of opensource software that solves opening and operationg big csv and dsv files.

# DSV Schema

DSV Schema describe the shape and typing of a csv file

The following csv files may be described as in the Schema:

File:

```csv
id;name;price;category
18280;apple;16.7;fruit
737;batmeat;8980.8;illegal
3432;;23.4;
12;toast;bakedGoods
```

Schema as csv:

```csv
header;type;colRequired;valRequired;misc
id;integer;true;true;
name;string;true;false;
price;float;true;false;default=0
category;enum;true;false;values=fruit,illegal,bakedGoods
```

Types:

- interger => -N until +N i.e. 1263
- floats => -N.n until +N.n i.e. 43.566473
- string => any string
- enum => allowed values, if valRequired==true then an empty values is alo allowed


