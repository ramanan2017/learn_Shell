# learn_Shell

We are Learning Shell script
list of Shell topics

1) Printing
2) Variables
3) Conditions
4) functions
5) Loops
6) SED Editor

##### SED Editor

1) Delete a line
2) Add a line
3) Change a line
4) Search and replace a word

#### SED is available in two form 
1) Display the changes on screen
   sed 'ACTION' FILE
2) Edit the file
   sed -i 'ACTION' FILE

#### Action Criteria can be picked in two ways.
1) Line Number based
2) String search based

Example:
If we want ti delete a line
For line number criteria  ==> sed '1 d' file  [ it will only show the delete file but actually will delte]
to Delete permanently     ==> sed -i '1 d' file [ will delete permanently]
For search string criteria ==> sed '/root/ d' file

cd /tmp
cp /etc/passwd .
ls
cat passwd
sed '1d' passwd
cat passwd
sed -i '1d' passwd
cat passwd
sed -i '/nologin/ d' passwd
cat passwd
sed '1 i Hello World' passwd
sed '/bash/ i Hello World' passwd
sed '/bash/ a Hello World' passwd
sed '/bash/ c Hello World' passwd
cat passwd
sed 's/halt/poweroff/' passwd
sed 's/halt/poweroff/g' passwd
sed 's/bash/BASH/' passwd
sed 's/bash/ksh/' passwd
sed '/roboshop/ s/bash/ksh/' passwd




