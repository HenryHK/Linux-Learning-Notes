# Files and Directories Management

## Create and Delete

```shell
# create dir
mkdir
# delete dir
rm
# delete non-empty dir
rm -rf
# delete logs
rm *log # the same as find ./ -name "*log" -exec rm {}
# move
mv
# copy
cp
# copy dir
cp -r
```

to see how many files under current path

```shell
find ./ | wc -l
```

to copy a directory

```shell
cp -r source_dir dest_dir
```

## switch path

```shell
# go to
cd
# go the last di
cd -
# go to home folder
cd ~
# display current path
pwd
```

## list files in dir

```shell
# list all files
ls
# list all files and display it in time order
ls -lrt
```

actually, for the frequent use of this command, we can set alias in `.bashrc`

```shell
alias lsl='ls -lrt'
alias lm=;;'ls -al|more'
```

## find dir and files