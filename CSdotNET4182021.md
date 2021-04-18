# CSdotNET4-18-2021
* namespace
* attribute
---
I am obsessed to body modification one day we could decide wether or not to rest or go on with tech replacement into this temporary shell. 
###  🤪 Array ```[]```, List```<T>```
> ```Array``` is fixed size collection, it neither add up nor remove its data\
> while ```List``` is more efficient to use in general it more flexible 
```cs
// define array
int[] Arr = new int[4] {1,2,3,4}
// define list
List<int> List1 = new List<int>{5,6,7,8}
```
---
### 🤪 interface, type
> Ideally ```interface``` is quite similar to ```type``` of property or method\
> but interface is used only for ```class``` and ```struct```\
> since class has no returning thing so```interface``` doesn't shape returning value but it does shapen class property and method for whatever declare in ```interface``` **MUST** declare in those ```class``` or ```struct``` as well
> ```interface``` is different from ```type```\
> ```type``` is **must be that ```type``` notion**\
> ```interface``` is **must implement that interface on whatever it apply to**
> So a class, property or method could have both type and interface at the same time.
```cs
	interface IRobot {
    	void getId();
        string Name {get; set;}
    }
    class Robot : IRobot {
    	//getId method is required due to this class implement on IRobot interface 
    	public void getId() => Console.WriteLine("My id is 0");
        // Name must be declare in this class due to its interface
        public string Name {get; set;}
    }
```
---
### 🤨ASP.NET Pipeline, routing ?

---
### 🤨Attribute
> ```attribute``` is metadata that attach to any particular object to chnage its behavior at ```Runtime```\
> there are 2 types of attribute ```Pre-defined``` and ```Custom one```
---
### 🤨```EF``` Entity Framework
> ```EF```is Object Relational Mapping or```ORM```\
> Object and Relational database are two different thing to implement those two, Object Relational Mapping comes in.\
> C#/.NET is ```OOP``` or purely class and object instance things, and SQL is relational data\
> So imlement these thing together could take a lot of work to get job done without using ```EF```\

Workflow:
1. ```Model``` for mapping Data into Database and vice versa.
2. ```Context``` is the database connection
3. ```Migration``` is ```LINQ``` codebase for actually insert/Interact data into Database. in the another word ```code``` in ```Migration``` translate into ```SQL``` language to dealing with database
---
### 🤨 ```MVC``` Design Pattern
> ```Controller``` is the center for interacting with ```View``` and ```Model```\
> ```View``` and ```Model``` aren't directly interact with each other
---