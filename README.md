
# PyTool-Kit 

**PyTool-Kit** is an Python tools. It contain many *usefull Tools*

## what is Pytool-kit 
PyTool-kit , its has Many tool for Python. This tool is use in everytime in Program(Python). But import this module for this and " *make progam small and easy to Understand*"

# Installation
Open **CMD**
![](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
``` bash
pip install pytool_kit
```
![](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
``` bash
sudo pip3 install pytool_kit
```
# Tools/Function
**Note:-**   Before use import moduls like below way :
``` python3
import pytool_kit as kit
```


## get_txt_between
 
This tool is use For, Get txt/string between the txt/string from txt/string that we want ...

### Example
This string(or txt) From Terminal (ifconfig)
``` python3 
inet6 fe80::d0f1:608c:a48b:5ab  prefixlen 64  scopeid 0x20<link>
inet 192.168.x.x  netmask 255.255.255.0  broadcast 192.168.0.255
ether 70:f1:a1:de:06:00  txqueuelen 1000  (Ethernet)
```
![](https://raw.githubusercontent.com/prajwalkedari/PyTool-Kit/main/img/get_txt_between.png)
From above txt File we Want *ip address* in 2 second Line , we Known that **ip is between inet & netmask** 
``` python3
parse1 = "inet" 
parse2 = "netmask"
text_var = txt/string 
kit.get_txt_between(text_var,parse1,parse2)
```
### output
```
192.168.x.x
```
## add_txt_between
this tool use for , txt(string) add in txt(string) or replace 

### example
```
txt = "Ben is an Girls who live in his "
```
now we add or replace *Girls By boy* is between a **" is an "** and  is an  is an **" "who live**
![](https://raw.githubusercontent.com/prajwalkedari/PyTool-Kit/main/img/add_txt_between-img.png)
```
parse1 = "is an" 
parse2 = "who live"
text_var = txt/string 

#add/replace

kit.add_txt_between(txt,"boy",parse1,parse2) 
>>>Ben is an boy who live in his


#replace txt from parse2 to end as "add this from kit" (parse2=" ")

kit.add_txt_between(txt,"add this from kit ",parse1, " ")
>>>Ben is an girls add this from kit


#replace txt starting to parse1 to "add this from kit" and parse2 as it is(parse1=" ")

kit.add_txt_between(txt,"add this from kit ",parse1, " ")
>>>Ben is an girls add this from kit

```
## txt2array
 
 This tool is convert it convert txt to array
### Example
```
string = "Python is an interpreted high-level general-purpose programming language"
```
now it convert to array

```
kit.txt2array(string)
>>>{'Python', 'is', 'an', 'interpreted', 'high-level', 'general-purpose', 'programming', 'language'}
```
## array2txt
this tool is use from convert Array to Txt(string)
### Example
```
array_test = {'A', 'computer', 'is', 'a', 'machine'}
```
now, It convert to simple txt or (string)
```
kit.array2txt(array_test)
>>>A computer is a machine 
```
## array2dic
This tools use for Convet Two array to one Python Dictory
### Example
```
Name = ["Prajwal", "Ram" , "Rohit" , "Subodh" ,"Pratham"]
Marks =[95,68,58,81,70]
```
There are Two array (Name and Marks) than convert To Dictory
```
kit.array2dic(Name,Marks)
>>>{'Prajwal': 95, 'Ram': 68, 'Rohit': 58, 'Subodh': 81, 'Pratham': 70}
```
## dic2array
dic2array tool use for Conervet 1 Dictory into 2 array
## Example
```
dict={'Prajwal': 95, 'Ram': 68, 'Rohit': 58, 'Subodh': 81, 'Pratham': 70}
```
Now,THis Dictory convert to 2 array <br>
**Note:-** it  return three array <br>
1 =>key value <br>
2 =>item value <br>
3 => key and they value <br>
```
a,b,c=kit.dic2array(dict)

#its Take varibale a,b and c resptivly

a
>>>(['Prajwal', 'Ram', 'Rohit', 'Subodh', 'Pratham'], 

b
>>>[95, 68, 58, 81, 70], 

c
>>>[('Prajwal', 95), ('Ram', 68), ('Rohit', 58), ('Subodh', 81), ('Pratham', 70)])
```

## License
[![](https://img.shields.io/github/license/prajwalkedari/wifi-password?style=plastic)](https://github.com/prajwalkedari/Pytool-kit/blob/main/LICENSE)
## Requirement

![](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) 

Install python3 on pc:-

![](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

  
## 🔗 Links
[![linkedin](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/prajwalkedari/Pytool-kit)
[![Gitlab](https://img.shields.io/badge/GitLab-330F63?style=for-the-badge&logo=gitlab&logoColor=white)](https://gitlab.com/PrajwalKedari/pytool-kit)
[![Bitbucket](https://img.shields.io/badge/Bitbucket-0747a6?style=for-the-badge&logo=bitbucket&logoColor=white)](https://bitbucket.org/prajwalkedari/pytool-kit)
