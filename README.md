
# project4




































































mkdir g
git --version
git config --list
git config --global user.name "Dimal"
git config --global user.email "Dimal"
ls -la

git add .
git status
git reset 1.txt
git commit -m "1.txt created"
git log --oneline
git log --author "Dimal"
git rev-parse --verify HEAD
git diff
git rm 2.txt
git mv 1.txt 11.txt
git commit --amend    - To edit the recent commit


git branch
git branch feature1
git checkout feature1
git diff master feature2
git branch -m feature2 feature22
git branch -d feature1
git merge feature22
git reset HEAD~
git reveret abs567ddnghgjkkd243

git remote -v
git remote add origin https://github.com/dimalmathew/p1.git
git remote remove origin
git push -u origin master --allow-unrelated-histories
git pull origin feature1

git stash save "2.txt updated but not saved"
git stash list
git stash show stash@{0}
git stash show -p stash@{0}
git stash pop stash@{0}
git stash apply
git stash drop stash@{0}
git stash clear



------------------------
read -p 'Enter number 1 : ' a
s=$(($a+$b))
div=$( echo "scale=3;$a / $b" | bc)
rev=$( echo "$str" | rev)


if [ "$str" == "$reverse" ]
then
	echo "Palindrome"
else
	echo "Not palindrome"
fi


if(($a>$b))
then 
	if(($a>$c))
	then
	l=$a;
	else 
	l=$c
	fi
elif(($b>$c))
then
	l=$b
else
	l=$c
fi



for((i=1;$i<=$n;i++))
do
f=$(($f*$i))
done



while((n>0))
do 
t=$(($n%10))
s=$(($s+$t))
n=$(($n/10))
done


while :
do
	echo "enter your choice"
	read c
	case $c in
	1)
		echo "1"
		read enterkey;;
	2)
		echo "2"
		read enterkey;;
	0)
		echo "exiting"
		exit 1;;
	*)
		echo "enter valid operator"
		read enterkey;;
	esac
done

read -p 'Enter the filename : ' filenm
array=( $(find . -name $filenm\* -print) )
temp=${#array[@]}
if [[ $temp > 0 ]]
then
for i in ${array[@]}
do
    extension="${i##*.}"
echo $extension
done
else
	echo "No file conatining with name    $filenm   exist"
fi
