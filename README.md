# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1

![image](https://github.com/user-attachments/assets/f94ff525-9416-4b40-b798-f779efb4a384)


cat > file2

![image](https://github.com/user-attachments/assets/0e568b0f-a3e9-441e-a50e-881e8093a35a)


### Display the content of the files
cat < file1
## OUTPUT

![image](https://github.com/user-attachments/assets/91d0f238-1e48-4f4d-ba90-c32963a3fde0)


cat < file2
## OUTPUT
![image](https://github.com/user-attachments/assets/31b14166-984c-4559-99b1-e1f5a1558acf)


# Comparing Files
cmp file1 file2
## OUTPUT
 ![image](https://github.com/user-attachments/assets/180510cf-0d9b-41f3-b845-91da00b0a92d)

comm file1 file2
 ## OUTPUT
![image](https://github.com/user-attachments/assets/5c7f5f92-ff66-4891-8f90-1d63a190fd16)

 
diff file1 file2
## OUTPUT

![image](https://github.com/user-attachments/assets/769c6019-9f78-4e39-889e-1bccd31192eb)

#Filters

### Create the following files file11, file22 as follows:

cat > file11
![image](https://github.com/user-attachments/assets/d4a75995-434c-47f3-b740-5fa5776f4f61)

cat > file22
![image](https://github.com/user-attachments/assets/3ddb9921-c790-49c8-8e98-c0d1c3cef654)



cut -c1-3 file11
## OUTPUT

![image](https://github.com/user-attachments/assets/56d289d7-3d5b-4eab-ab44-d1938a3cd20b)



cut -d "|" -f 1 file22
## OUTPUT

![image](https://github.com/user-attachments/assets/869160f5-41eb-46b7-89dd-0a0672bb956f)


cut -d "|" -f 2 file22
## OUTPUT
![image](https://github.com/user-attachments/assets/95e8d1e9-a58b-42fb-bbf5-ddd7e31bc4c6)


cat < newfile 
![image](https://github.com/user-attachments/assets/83f62a29-0980-4b6d-9677-0a50e18593c9)

cat > newfile 
![image](https://github.com/user-attachments/assets/38828db4-910e-4ebc-a4c5-aecf514f70d1)

 
grep Hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/4ae7d08d-058f-4172-8b74-89012c08ea65)


grep hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/ea99013d-e874-49b0-810d-94915dd656df)



grep -v hello newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/e854c1c3-0191-4af5-a862-49e9a54c8ce7)


cat newfile | grep -i "hello"
## OUTPUT

![image](https://github.com/user-attachments/assets/47296e01-47d9-4933-8aaa-6df2099cd17e)



cat newfile | grep -i -c "hello"
## OUTPUT

![image](https://github.com/user-attachments/assets/975f15c5-3c75-408d-bb27-23471519d327)



grep -R ubuntu /etc
## OUTPUT

![image](https://github.com/user-attachments/assets/91b1ad17-ed91-46a7-a22b-57305819e612)


grep -w -n world newfile   
## OUTPUT

![image](https://github.com/user-attachments/assets/8a8bf949-b763-4791-a4a7-80b56ea96efc)

cat < newfile 
```
Sanjit anand
sanjit anand
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

cat > newfile
![image](https://github.com/user-attachments/assets/e2b4c107-e4a7-42e2-b1eb-e49877fe5478)


egrep -w 'Hello|hello' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/563bc518-3501-4012-8242-3f3738c7d3ef)



egrep -w '(H|h)ello' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/ee7a602e-0513-40c9-938e-24c718df8b38)



egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/b598609c-48a9-4042-9f6a-6116d90654c1)


egrep '(^hello)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/fbd3e8b6-3acb-4931-b305-8847d24fd738)


egrep '(world$)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/8e39c91b-6ba1-41b8-b23f-9e3ccc3a9bf2)


egrep '(World$)' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/3e0edf43-a63c-40fc-b4ed-b07e7391fedc)


egrep '((W|w)orld$)' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/6bbefd3d-4e96-44a9-ab69-553600a1c3c6)


egrep '[1-9]' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/99a618db-9658-4466-b88d-019b36cae19d)


egrep 'Linux.*world' newfile 
## OUTPUT
![image](https://github.com/user-attachments/assets/664f4efd-abc8-4141-a30f-e1d63dcda9d5)


egrep 'Linux.*World' newfile 
## OUTPUT

![image](https://github.com/user-attachments/assets/45570e7e-5355-4541-84aa-b0a30d5ffc22)

egrep l{2} newfile
## OUTPUT

![image](https://github.com/user-attachments/assets/77b03b92-ab88-43a9-8ae5-66cae6f4581a)


egrep 's{1,2}' newfile
## OUTPUT 
![image](https://github.com/user-attachments/assets/1b90627a-451a-408d-b11f-1ea8aeb6f49d)


cat > file23
![image](https://github.com/user-attachments/assets/5c12135f-bd6a-4b53-99c8-fbcbf6c289f4)



sed -n -e '3p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/77536722-0ac0-4bed-b8f9-c10819f39d91)


sed -n -e '$p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/898e1af1-74bf-4fc6-9002-dcdc830095cb)


sed  -e 's/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/cee06147-ca82-4c5e-978b-a1057c6d24dd)


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/874bec26-f9a1-497f-ad15-b3964e1da7c7)


sed  '/tom/s/5000/6000/' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/f6fc4c47-5057-49a8-8057-59fa96b57105)


sed -n -e '1,5p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/89497324-a8f5-4300-b952-f1a6353abf07)


sed -n -e '2,/Joe/p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/9c666bc4-5761-4e4a-8edd-e1348218bdd3)



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/36af24c7-ea6a-4f32-acd4-fb5860e53022)


seq 10 
## OUTPUT

![image](https://github.com/user-attachments/assets/0e34bb26-62d3-4150-a1b8-d43b27b056c8)



seq 10 | sed -n '4,6p'
## OUTPUT

![image](https://github.com/user-attachments/assets/9ed1cfa7-d620-4371-bb82-5b320720156f)


seq 10 | sed -n '2,~4p'
## OUTPUT

![image](https://github.com/user-attachments/assets/518090cc-0d55-40e3-a976-3c7c674abcad)


seq 3 | sed '2a hello'
## OUTPUT

![image](https://github.com/user-attachments/assets/25232d77-f444-439a-9e3b-e562ec8999c1)


seq 2 | sed '2i hello'
## OUTPUT
![image](https://github.com/user-attachments/assets/66458bed-4225-433a-882c-7013eab9a08b)


seq 10 | sed '2,9c hello'
## OUTPUT
![image](https://github.com/user-attachments/assets/2454ed06-6f49-4f24-8d08-8d91b935aed8)


sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

![image](https://github.com/user-attachments/assets/326f4810-3b11-4232-b3a7-f4b5683191ca)


sed -n '2,4{s/$/*/;p}' file23
```
$1001 | Sanjit | 10000 |HR*
$1002 | tom | 5000 |Admin*
$1003 | Joe | 7000 |Developer*
```

#Sorting File content
cat > file21
![image](https://github.com/user-attachments/assets/b09a1aba-e545-4633-8131-eba33027bf9a)
 
sort file21
## OUTPUT
![image](https://github.com/user-attachments/assets/12e3fcc7-5e16-49c6-bbe0-a7ff89111698)


cat > file22
![image](https://github.com/user-attachments/assets/010e8ebd-9b36-4460-8eea-3705ee53566f)

uniq file22
## OUTPUT

![image](https://github.com/user-attachments/assets/fb10b0ca-2db2-47ad-86a2-d4c13c19b0c7)


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT
 ![image](https://github.com/user-attachments/assets/efdfd016-41f1-4c96-a780-36dba8c31d30)


cat < urllist.txt
![image](https://github.com/user-attachments/assets/b4ed2196-2db3-4c32-8884-fe650024c330)

cat > urllist.txt
![image](https://github.com/user-attachments/assets/92bc98b7-41b5-4c6d-84e5-b976bbc18f1d)

cat urllist.txt | tr -d ' '
 ## OUTPUT

![image](https://github.com/user-attachments/assets/771b349b-c361-48e0-8f40-0a8bc24f48ce)

 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

![image](https://github.com/user-attachments/assets/bcd22c35-9dd9-42f1-8c2b-3386147e0070)


#Backup commands
tar -cvf backup.tar *
## OUTPUT
![image](https://github.com/user-attachments/assets/0c2177ee-5f3f-405e-a70b-f437a45e40d3)


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar

-rw-r--r-- user/group 0 2024-02-25 14:30:00 file1.txt drwxr-xr-x user/group 0 2024-02-25 14:30:00 directory1/ -rw-r--r-- user/group 1024 2024-02-25 14:30:00 directory1/file2.txt -rw-r--r-- user/group 2048 2024-02-25 14:30:00 directory1/file3.txt tar -xvf backup.tar

# OUTPUT
x file1.txt x directory1/ x directory1/file2.txt x directory1/file3.txt gzip backup.tar

ls .gz

# OUTPUT
backup.tar.gz gunzip backup.tar.gz

# OUTPUT
backup.tar

# Shell Script
echo '#!/bin/sh' > my-script.sh echo 'echo Hello World‘; exit 0 >> my-script.sh
chmod 755 my-script.sh ./my-script.sh

## OUTPUT
![image](https://github.com/user-attachments/assets/099afd2b-9716-4982-8e0c-2f8e7f6bdee2)

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT
![image](https://github.com/user-attachments/assets/86a1546a-7f15-4763-82c9-230c932d40e0)


cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT
![image](https://github.com/user-attachments/assets/dd80df6c-3d47-4fae-b5c3-a792dd30e6a7)

 
ls file1
## OUTPUT
![image](https://github.com/user-attachments/assets/49ac433e-04e4-422e-b06b-084ba84a342e)

echo $?
## OUTPUT 
![image](https://github.com/user-attachments/assets/dc4c6a43-6472-4f3e-b6c6-caf5217efce6)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 ![image](https://github.com/user-attachments/assets/f8f7e8ac-e9d3-438c-ae57-7fbc324a4930)

abcd
 
echo $?
 ## OUTPUT
![image](https://github.com/user-attachments/assets/ca53a7cd-3f87-449f-89cc-47ffbb78d5c4)


 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/38fc7de2-98aa-4307-a66e-a9f771dcab21)

# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT
![image](https://github.com/user-attachments/assets/0f4aa794-2d1e-4fbf-a65c-ab7be5da8104)

# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi

```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/da4ee2de-b9b5-4835-b918-71e97396d3d8)


# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi

```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/7e2188d8-45f1-434c-85ae-53b6658391b8)


# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi

```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/9620faba-4b7f-401a-8daf-ec76a86b2263)

# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/579bd474-6dcd-4e1a-b3f4-5b035bc4ca2f)


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/585af7a5-c287-416b-8522-d488ba7e241b)

# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 

# Output
![image](https://github.com/user-attachments/assets/1867a9c8-48d4-4f80-8d79-e9ba5ed3b907)

 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh
 # Output
 ![image](https://github.com/user-attachments/assets/ebf045b5-fde2-4e53-b4d9-87f075a248d5)

 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
 
 # Output
 ![image](https://github.com/user-attachments/assets/61c58ac4-354d-4246-88b4-198c6499c520)

 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 # Output
 ![image](https://github.com/user-attachments/assets/e80d1d51-d6f1-4f63-a41f-052c477cd9aa)

cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
# Output
![image](https://github.com/user-attachments/assets/9a9a9a87-edc2-40d1-9086-83f0d25d8ee8)

 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT
cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT


cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/3aa17f34-38b1-42dd-b5c7-3fc4c8802e34)

cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT
![image](https://github.com/user-attachments/assets/aa73e4b7-6785-4e48-a7e4-bd94190a0ddb)

cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT
![image](https://github.com/user-attachments/assets/86ad3f84-6657-497f-b678-7560e2ac16e0)

 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT
![image](https://github.com/user-attachments/assets/707fc443-6f6a-43cd-9a72-63edf4a12fa2)

$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 ![image](https://github.com/user-attachments/assets/65b977a0-a1c5-4a34-ae7a-ce88e66b7472)

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

![image](https://github.com/user-attachments/assets/90b7b6f9-2d70-4e28-a7c2-541fa3acdf1d)

 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

![image](https://github.com/user-attachments/assets/e779af4c-399c-4165-b729-d938fcf07495)


$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT
 ./funcex.sh 
![image](https://github.com/user-attachments/assets/82147925-6774-4791-b12f-a856c66198f1)

 
 ./funcex.sh 1 2
 # Output
![image](https://github.com/user-attachments/assets/f51fcc44-d880-4f5d-8f24-78076f7d3a2c)

 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT
$ ./argshift.sh 1 2 3
 ![image](https://github.com/user-attachments/assets/2a3909c1-6b79-4cec-91a7-67918fa35894)

 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT
$ ./argshift.sh 1 2 3
 ![image](https://github.com/user-attachments/assets/3440f56c-3f82-4636-ada8-14434d33310c)

cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT
 ./argshift.sh 1 2 3
 
 ![image](https://github.com/user-attachments/assets/d227c479-eff8-4aa3-8655-a90b2de8332b)

cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 
 ![image](https://github.com/user-attachments/assets/b07b353f-dba4-438b-9937-858eb4c2f547)

cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 
![image](https://github.com/user-attachments/assets/0bd42060-11ed-4e35-a717-4443a6a36af2)


# RESULT:
The Commands are executed successfully.
