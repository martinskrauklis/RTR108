# RTR108
Studiju kursa Datormācība (speckurss) elektroniskā klade
## 2. nodarbība
rinda 1  
rinda 2  
rinda 3  

## 4. nodarbība
---------------------------------------------------------
Nodarbības laikā atkārtotas komandas, un to nozīme:  

uname  
operētājsistēma  

uname -a  
operētājsistēma, detalizēti  

echo $0  
lietotais interpretators  

pwd  
patreizējā mape  

whoami  
patreizējais lietotājs  

sh  
pārslēgties uz shell interpretatoru  

bash  
pārslēgties uz bash interpretatoru  

man <...>  
gūt aprakstu par konkrētas komandas darbību  

chmod  
failu piekļuves informācija  
tiek pierakstīta decimālajā sistēmā, kā  
pārveidojums no binārās (rwxrwxrwx)  

echo $PATH  
pārbaudīt, kurās mapēs tiek meklētas komandas  
lai pievienotu jaunu mapi komandu meklēšanai,  
jāvada PATH=$PATH:<šeit vadam mapes>. Svarīgi  
ir iekļaut šajā komandā "$PATH", pretējā  
gadījumā būs auzas, jo patreiz lietotās mapes  
tiks nodzēstas (komanda nevis papildina esošo  
sarakstu, bet veido no jauna).  


## 5. Nodarbība

Skripti iekš shell

Mainīgie drīkst sastāvēt no burtiem, skaitļiem 
un apakšsvītras, kā arī tiek ir jāsākas ar burtu.

Mainīgā_nosaukums = mainīgā_vērtība - ja vērtība
tiek piešķirta teksta veidā, to nepieciešams likt
pēdiņās. Ja šī vērtība ir skaitlis - tādā gadījumā
pēdiņas nav nepieciešamas.

readonly NAME - mainīgais NAME tiek saglabāts ar 
atribūtu "tikai lasāms".

unset NAME - mainīgais NAME tiek atiestatīts, tā
vērtība tiek iestatīta kā tukšums.

read NAME - tiek pieprasīta datu ievade, no kuras 
ievadītie dati tiek saglabāti mainīgajā NAME.

echo $NAME - tiek attēlots mainīgais NAME.

$0 - patreizējā skripta nosaukums.

$n - these variables correspond to the arguments with which a script was invoked. Here n is a positive decimal number corresponding to the position of an argument (the first argument is $1, the second argument is $2, and so on).
3 	

$#

The number of arguments supplied to a script.
4 	

$*

All the arguments are double quoted. If a script receives two arguments, $* is equivalent to $1 $2.
5 	

$@

All the arguments are individually double quoted. If a script receives two arguments, $@ is equivalent to $1 $2.
6 	

$?

The exit status of the last command executed.
7 	

$$

The process number of the current shell. For shell scripts, this is the process ID under which they are executing.
8 	

$!

The process number of the last background command.
