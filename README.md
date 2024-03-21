![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/8b856d3b-0923-4c98-b0f2-1f9047c621a0)# OS-Linux-commands-Shell-scripting
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
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/8d826f4f-5c02-4397-8754-742d054f20a7)

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f4b5ee19-22a5-4d43-9368-46eb73d4bf45)

### Display the content of the files
cat < file1
## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/aa3fbd68-ad6c-44b0-8eda-e3ee0d71f2f0)



cat < file2
## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/287ffb1f-7eda-4bc8-94b3-5d94a22b53d0)


# Comparing Files
cmp file1 file2
## OUTPUT
 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f1fbe37f-f73e-46d0-99ba-4e57dac57f19)

comm file1 file2
 ## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f8a1e416-be3a-42c5-b6f4-fe2ef97b44a1)

 
diff file1 file2
## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/1a74a219-0b91-4c01-89e7-0eeab25aee37)


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/0a1d3aa9-90c5-4e86-bed7-55ab72481321)

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/99bbb4e0-3692-4fcf-92b1-38bce98bb31d)


cut -c1-3 file11
## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/bc992536-4ea0-40e7-9ae9-b170cf132843)




cut -d "|" -f 1 file22
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/9dead051-1260-4d87-87a6-eb6df2b9df61)


cut -d "|" -f 2 file22
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/41befca4-e6bb-4358-8566-a983fe146669)

cat < newfile 
```
Hello world
hello world
^d
````
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/69a1d4f4-c9dc-4e66-b7a9-6c1b68d16af6)

cat > newfile 
Hello world
hello world
 
grep Hello newfile 
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/1f08bc02-3855-49b7-a099-bfe1a834d037)


grep hello newfile 
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/0837caf9-b302-4def-967a-6a7c8a5cdff6)

## OUTPUT

grep -v hello newfile 
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/412b8aa3-1325-4af4-9c33-4ba1dbba8656)

## OUTPUT

cat newfile | grep -i "hello"
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/b0a71a5f-b56b-4620-ae84-99bfaad1564d)


## OUTPUT


cat newfile | grep -i -c "hello"

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/ce2b6bc9-bc37-4482-9b5b-5521ebbb1079)


## OUTPUT

grep -R ubuntu /etc

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/15de3872-2de7-4426-9e63-4301478e837b)

## OUTPUT

grep -w -n world newfile   

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/df782e7c-5520-43ed-b0b7-2cbe20353963)

## OUTPUT


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/b5f1c1aa-5498-49a0-b5a3-e70a91a3fb4c)

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/d1ffb5ab-0861-45ce-8599-522c5c670cae)

egrep -w 'Hello|hello' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/9278287d-f25e-402f-9d16-13ce6536c373)

## OUTPUT


egrep -w '(H|h)ello' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/79eccf46-a367-49c4-b580-edb58aef3c31)

## OUTPUT

egrep -w '(H|h)ell[a-z]' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c9246fbb-06b7-401b-9ca1-f3a46c0180b9)

## OUTPUT

egrep '(^hello)' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/e5157ede-d9bd-4a4d-96e4-4524b06fa0d2)

## OUTPUT

egrep '(world$)' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/7801cf68-847a-489f-acc9-243030933e08)

## OUTPUT

egrep '(World$)' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/eec6b232-40fc-4ef3-8a9f-ce904245e72c)

## OUTPUT

egrep '((W|w)orld$)' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/2eed71f6-d689-48de-bc9a-9ecb7f0dc25b)

## OUTPUT



egrep '[1-9]' newfile 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/250e4979-ffbf-4a36-a527-bd9428a396a3)

## OUTPUT



egrep 'Linux.*world' newfile 
## OUTPUT


egrep 'Linux.*World' newfile 
## OUTPUT


egrep l{2} newfile

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/6a512571-4172-43b7-9bb0-96ecb8b4473c)

## OUTPUT



egrep 's{1,2}' newfile

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/7fe6fe49-9a16-4cb8-a159-342a0adb16a3)

## OUTPUT 


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/e134bdad-8b94-49b1-b06e-b033e540fed2)


sed -n -e '3p' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/9230cd8e-9c85-44de-ab31-479db5a01089)

## OUTPUT



sed -n -e '$p' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/6a35f019-5cdc-4f63-a617-75003277625d)

## OUTPUT



sed  -e 's/Ram/Sita/' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/095a5edc-eda2-42c8-9a06-f5c9f83b7a15)

## OUTPUT


sed  -e '2s/Ram/Sita/' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/293c5747-8b19-4f45-ab42-cd24cdcacc2e)

## OUTPUT



sed  '/tom/s/5000/6000/' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c611f39b-012c-4923-8f1e-be1261ac3b0e)

## OUTPUT



sed -n -e '1,5p' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/174a53cf-3083-48aa-bf15-aa81997c53ee)

## OUTPUT



sed -n -e '2,/Joe/p' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/47d896cd-ec9b-4f5f-ae81-de87afc0bead)

## OUTPUT




sed -n -e '/tom/,/Joe/p' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/da0a325e-dbe5-47d3-ad18-366965f3cbc3)

## OUTPUT



seq 10 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/cef77d40-7cc2-4ffc-8b8e-ac829b3e0a0a)

## OUTPUT



seq 10 | sed -n '4,6p'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/6f5f7510-d03d-4702-8c3d-9d61e69112cf)

## OUTPUT



seq 10 | sed -n '2,~4p'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/cb7d61f8-5352-4a9a-9281-f5aa8b29823a)

## OUTPUT



seq 3 | sed '2a hello'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/010818e8-276f-4bb6-98db-a8faa28c7cb1)

## OUTPUT



seq 2 | sed '2i hello'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/8e4fd4d8-7c4c-479f-833d-391d8d4c0880)

## OUTPUT


seq 10 | sed '2,9c hello'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/b52c8bac-b018-42aa-8407-fa4b2a66fe0c)

## OUTPUT


sed -n '2,4{s/^/$/;p}' file23

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/df26b22d-e94c-4e92-a9ab-b4ee22722403)

## OUTPUT



sed -n '2,4{s/$/*/;p}' file23




#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT


cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT


 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT



#Backup commands
tar -cvf backup.tar *
## OUTPUT


mkdir backupdir
 
mv backup.tar backupdir
 
tar -tvf backup.tar
## OUTPUT


tar -xvf backup.tar
## OUTPUT

gzip backup.tar

ls .gz
## OUTPUT
 
gunzip backup.tar.gz
## OUTPUT

 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT


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
^d
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

 
ls file1
## OUTPUT

echo $?
## OUTPUT 
./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 
 
abcd
 
echo $?
 ## OUTPUT


 
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
^d
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
##OUTPUT



chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT


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
^d
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
^d
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
^d
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
##OUTPUT

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
^d
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
##OUTPUT

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


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT



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

 
 ./funcex.sh 1 2

 
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


# RESULT:
The Commands are executed successfully.
