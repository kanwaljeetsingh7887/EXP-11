# EXP-11

## Aim:
**To study and implement Classes and Objects..**

## Software:
`Microsoft VSCode`

## Theory:
Class -> A class is a usser-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class.

Object-> When a class is defined, only the specification for the object is defined, no memory or storage is allocated. To use the data and access functions defined in the clss, we need to create objects.

In C++, there are three access specifiers that are:
(1) Public: Members declared as public can be accessed from outside the class.
(2) Private: Members declared as private can only be accessed within the class itself.

(3) Protected: Members declared as protected cn be accessed within the class and by derived classes.
Any changes made to the parameters within the function are directly reflected in the original values outside the function.
## Code: 11A
```
//KANWALJEET SINGH
//ENTC B2
//EXP 11A
//23070123124
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0;
    double b = 3.0;
    double l = 4.0;
};
int main()
{
  cuboid c1;
  double vol = c1.h * c1.b * c1.l;
  cout<<"Volume "<<vol<<endl;
}
```
## Output:
![image](https://github.com/user-attachments/assets/d07f645f-c40e-4673-9956-287322b33156)







## Code: 11B
```
//KANWALJEET SINGH
//ENTC B2
//EXP 11B
//23070123124
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0,b = 3.0,l = 4.0;
    double volume()
    {
        double vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```

## Output:
![image](https://github.com/user-attachments/assets/094f37b8-9ccf-4a88-a838-f98fff3ba791)



## Code:11C
```
//KANWALJEET SINGH
//ENTC B2
//EXP 11C
//23070123124
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 3.0,b = 2.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```

## Output: ![image](https://github.com/user-attachments/assets/87c9c5e6-1796-42c1-b373-0ee41ca0eb4b)


## Code: 11D
```
//KANWALJEET SINGH
//ENTC B2
//EXP 11D
//23070123124
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 2.0,b = 3.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    double v = c1.volume();
    c1.disp(v);
  
}
```

## Output: ![image](https://github.com/user-attachments/assets/6b0cb225-f643-4c62-9605-56e8deae4b22)


## Code: 11E
```
//KANWALJEET SINGH
//ENTC B2
//EXP 11E
//23070123124
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h,b,l;
    void input()
    {
        cout<<"Enter the length: ";
        cin>>l;
        cout<<"Enter the breadth: ";
        cin>>b;
        cout<<"Enter the height: ";
        cin>>h;
    }
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    c1.input();
    double v = c1.volume();
    c1.disp(v);
  
}
```
## Output: ![image](https://github.com/user-attachments/assets/fcabb536-3c91-4717-a564-bf681fdeb41f)



### Conclusion:
In this experiment, i learnt about classes and objects in C++ and performed programs using them and also learnt about local variables and global variables.
