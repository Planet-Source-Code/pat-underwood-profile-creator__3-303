<div align="center">

## Profile Creator


</div>

### Description

It asks you name, age, height, etc. and puts them in a *.txt file...
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Pat Underwood](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/pat-underwood.md)
**Level**          |Beginner
**User Rating**    |3.7 (26 globes from 7 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Complete Applications](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/complete-applications__3-7.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/pat-underwood-profile-creator__3-303/archive/master.zip)

### API Declarations

iostream.h, ofstream.h


### Source Code

```
#include <iostream.h>
#include <fstream.h>
/////////////////////////
//Made By Pat Underwood//
//http://patu.iwarp.com//
/////////////////////////
int age, heightin, heightft;
char firstname[30];
char lastname[30];
char gender[7];
ofstream foo("profiles.txt");
void main () {
//Start questioning
cout << "Enter your first name:\n";
cin >> firstname;
cout << "Enter your last name:\n";
cin >> lastname;
cout << "Enter your gender (male or female):\n";
cin >> gender;
cout << "Enter your age:\n";
cin >> age;
cout << "Enter your height (feet only) :\n";
cin >> heightft;
cout << "Enter your height (inches only) :\n";
cin >> heightin;
//Start confimation
cout << "-" << firstname << lastname << "\n";
cout << "-" << gender << "\n";
cout << "- Age = " << age << "\n";
cout << "-" << heightft << "' " << heightin << "''\n";
foo << "Name: " << firstname << " " << lastname << "\n";
foo << "Gender/Sex: " << gender << "\n";
foo << "Age: " << age << "\n";
foo << "Height: " << heightft << "' " << heightin << "''\n";
cout << "Thank you, your new profile is being created...\n";
cout << "This program was made by Pat Underwood, you can get more of his software at \nhttp://patu.iwarp.com\n";
}
```

