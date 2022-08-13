# Fixing pendrive showing less total memory that its actually capacity

Sometimes windows cannot recognize a partition on a pendrive when there are more than one partitions.

Source [extra stuff](https://www.partitionwizard.com/resizepartition/64gb-flash-drive-only-showing-32gb.html)

* open cmd and run the commands belows

```bash
diskpart
```

```bash
list disk
```
this will list all the internal and external disk on the machine with a naming scheme as Disk 0, Disk 1 so on.

Select the pendrive by the following command

```bash
SELECT DISK={number of the disk 0/1/2 whatever in the Disk### column}
```

The pendrive will be selected

now run a command to clean the pendrive

```bash
clean
```

```bash
create partition primary
```

now the next command formats the pendrive so backup the data if its important

```bash
format fs=ntfs quick
```

the pendrive will be formatted and it will now show the original capacity of the pendrive.


