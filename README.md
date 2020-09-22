<div align="center">

## Beginner Examples \- how to format output


</div>

### Description

A couple of simple examples of ways to format output using iomanip; ie: set width, right align, left align, change fill character
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[\*LuckY\*](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/lucky.md)
**Level**          |Beginner
**User Rating**    |4.0 (16 globes from 4 users)
**Compatibility**  |C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/lucky-beginner-examples-how-to-format-output__3-931/archive/master.zip)





### Source Code

```
#include <iostream>
#include <iomanip>
using namespace std;
//
int main() {
	/*notes: newer implementations use ios_base
	and not ios. Also they allow using the following
	syntax:
		cout << left;
	to set the alignment to the left/right
	*/
	//
	cout.setf(ios::left,ios::adjustfield);
	cout << setw(20) << "Name:";
	cout.setf(ios::right,ios::adjustfield);
	cout << setw(60) << "Occupation:\n";
	//
	/* change fill character from ' ' to '.' */
	//
	cout.fill('.');
	//
	cout.setf(ios::left,ios::adjustfield);
	cout << setw(20) << "*LuckY*";
	cout.setf(ios::right,ios::adjustfield);
	cout << setw(60) << "Student -- Computer Science\n";
	//
	return 0;
}
```

