# Seek Help in Linux

## See brief instructions of command

```shell
whatis <command>
```

or use regular expression

```shell
whatis -w "loca*"
```

to see more detailed instructions

```shell
info <command>
```

## `man`

```shell
man <command>
```

there are 9 categories in `man`. Some keyword may exist in multiple categories, we should declare certain categories to get instructions we desired. (In general, bash command is listed in category 1)

The `whatis` command mentioned above can show categories of specific command. e.g.

```shell
whatis printf
printf               (1)  - format and print data
printf               (1p)  - write formatted output
printf               (3)  - formatted output conversion
printf               (3p)  - print formatted output
printf [builtins]    (1)  - bash built-in commands, see bash(1)
```

if someone want to see the usage of `printf` in C, he should type

```shell
man 3 printf
```

one can use `man -k keyword` to search commands containing the keyword.

```shell
man -k GNOME config | grep l
```

## Find Path

look for where binary file is

```shell
which command
```

look for the search path of one specific software

```shell
whereis command
```

used when there is multiple versions of one software.