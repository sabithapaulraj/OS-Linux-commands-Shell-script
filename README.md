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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/9ef530b7-6b86-442c-a1c4-f6aec9402f59)





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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/51a6dc04-72ce-4349-b94e-f47c4abb8014)


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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c0f8194d-93a1-4c95-8f9e-2fdc46592491)

## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/e90ed644-bb87-4d12-889f-58b7f744eb7a)



#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/a3cbf45a-24b2-44b1-8855-20885e218ca5)


cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/71b8e09a-f7fe-4796-9f6a-331fd1daddac)

cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c3a1cbef-00bc-461d-bdda-f7fb5b830f8f)

cat urllist.txt | tr -d ' '

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/e9b48bf2-dc38-4fd9-8eea-77d3a153342e)

 ## OUTPUT

cat urllist.txt | tr -d ' ' | tr -s '.'

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/912fb2e9-1670-4c02-844d-7cca8b4b027f)

## OUTPUT



#Backup commands
tar -cvf backup.tar *
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/29be9ead-732f-4a74-ab4d-22209845a4e6)



mkdir backupdir
 
mv backup.tar backupdir

 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/daa028aa-423f-4c58-82af-9c8335cfa77d)

tar -tvf backup.tar

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f17b5715-a691-4630-9b81-fff64bd9a586)

## OUTPUT


tar -xvf backup.tar

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/6412aa5a-e79b-4dee-9c8b-0cc6298aac0f)

## OUTPUT

gzip backup.tar

ls .gz

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/13e12f3c-423d-4d58-801a-15be45bae86d)

## OUTPUT
 
gunzip backup.tar.gz

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/fec89559-c8d1-4e2d-a4b3-59fbca4db0a6)



 
# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/b482cca7-8962-4860-b090-01c2f7d5631f)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/1b3717e7-816c-4559-9162-ba1bcc381389)

cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/8d87f8c1-ec1f-40bf-ae3d-a238cdae7f1e)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/bb580d5e-9d98-4bd4-9772-907f5a493a7b)


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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c588b9fa-70fb-46e2-b813-890537ed1ed3)


![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/2e16bd60-d505-4007-b33f-56db9624a4e9)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/5231a559-d457-4144-9049-3cc26942878f)

ls file1
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/1afa9eff-1dd2-4cb6-9c04-0f1a5c4dbaad)

echo $?
## OUTPUT 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/2e61fc4c-c3cc-4d53-8ac2-8699b8848d6b)

./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 

 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f75d0aeb-bed2-4131-8d09-0354e339aed0)

abcd
 
echo $?
 ## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/b2683246-7732-419a-9aa6-9b83bd1a3f62)


 
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
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/f9c4c7d3-3f51-4654-96c8-1089fd444799)




chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c3e6a3d1-5768-47df-bb8e-b4d5e1ee6f6a)



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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/4bc0833c-4767-48eb-b442-f8de40d1ba95)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/a9f06f33-d615-494c-aeeb-772da14700cd)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/387b2b9f-6946-482f-9a13-5cdefbcbdd1a)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/055e38c0-5d0e-442e-9a36-59c4797fd3e1)



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
## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/483b0887-bd1e-4eb6-9591-08ecec1fc41e)
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/03f55e4e-a4a2-4e90-9c0b-87b39075f66e)



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
## OUTPUT
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/325ec43b-4197-462d-94c4-9d9657961af2)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/83a0241b-4020-430b-9a7a-202965b054f5)

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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/bcc634bc-5954-4232-90aa-05be0d3d1ca0)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c4c90885-c2f1-4718-ae16-65a530a98edc)

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


![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/a41b9a13-0f5e-42d0-a411-0fb590cd5671)

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
 
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/71cc9ac9-051e-4f13-bfb3-ec66612cee3f)

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
 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/15ebf32c-fbd1-4e33-8530-7b77bd53c75d)

 
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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/9130f11b-7819-4a41-8fd4-57cff80b6ca9)
$ chmod 755 untiltest.sh
 
cat forin1.sh 
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/87df45c8-b2a7-4cbd-897b-e024ec0c1de0)

```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/0a3743d0-8c59-4c10-bf0e-2cd411f5a494)

$ chmod 755 forin1.sh
 
 
cat forin2.sh 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/60624a1d-3322-40f2-a790-f3ee3a89485f)

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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/5db7c59d-3bfc-4284-822d-d06f00ff1435)

 
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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/7701db5e-5306-425a-9d5d-012edd323a05)

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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/587f8b75-9e7b-42fb-abe6-ee595a8aa805)

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/8b1fd7ea-f2b6-43ca-9197-6f6036c19ac2)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/7ec1f0ea-f930-4b88-aeeb-a1258e80f53a)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/385006b9-d49d-465c-a1d5-0e996d06fcb5)

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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/24658c9b-c66b-4fe2-9eb2-a556f73de444)

 
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


$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/24fe1758-0ec0-41b7-8fa5-ca31c39c85b1)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/6a9303d1-a881-47ed-bd9d-099ef3c21dbc)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/85ce33d2-6012-4571-ab07-2cfa54eb95f0)


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/57b56712-3e10-4abe-ab75-ddd1b0f1f04a)



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
 
 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/ebd3ec88-ada0-4d86-b1e5-abe28f1a6b7a)

 
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


![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/ccb7ee05-e9c1-4592-92ec-6f67e8b7f853)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c736a718-56b3-4417-a87c-f86a1c6a818f)

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
 
 ![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/c29ad95b-c169-4ff1-8f0e-74b6f1c15b00)

 
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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/d7850997-0a34-4786-a55a-9f89853f7664)

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
![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/af6b4b57-0562-4499-bdeb-970163211290)

awk -f nc.awk data.dat
## OUTPUT 


![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/2774c0cd-c926-4206-8350-29d39440505c)

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

![image](https://github.com/sabithapaulraj/OS-Linux-commands-Shell-script/assets/118343379/37b5c6c2-d570-451c-bd4a-9fb00b0c8ef2)


# RESULT:
The Commands are executed successfully..
