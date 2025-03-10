# **DataStructures-And-Algorithms**

## **Data Structures :-**

### **Data Structures is a way of storing/organising data in the memory, in such a way that access, management and modification become efficient.**

## **Algorithms :-**

### **Algorithms is any approach you use to perform operations on data (like searching, sorting, traversing, ..Etc.).**

<hr>

# **Prerequisites :-**

0. **PROGRAMMING LANGUAGE.**
1. [**CLASS AND OBJECTS.**](https://youtu.be/a199KZGMNxk?t=244)
2. [**CONSTRUCTOR.**](https://youtu.be/a199KZGMNxk?t=981)
3. [**this KEYWORD.**](https://youtu.be/a199KZGMNxk?t=1424)
4. **ACCESS MODIFIERS IN JAVA.**

- ## **Public-** The access level of public modifier is everywhere. Methods, variables declared public can be accesed from anywhere after importing that class.
- ## **Default-** The access level of default modifier is within package. Methods, variables declared default can be accesed from other classes of same package.
- ## **Private-** The access level of private modifier is within the class. Methods, variables declared private cannot be accesed from outside the class.

5. [**ENCAPSULATION.**](https://youtu.be/a199KZGMNxk?t=2019)
6. [**STATIC KEYWORD IN JAVA.**](https://youtu.be/3LtIk7wFGi0)
7. [**INNER CLASS IN JAVA.**](https://youtu.be/zg1pijw6AM4)
8. [**Pass by value.**](https://youtu.be/H71vRa86AGg)
9. [**Pass by refrence.**](https://youtu.be/H71vRa86AGg)

```java
import java.util.*;

public class Hi {

	// here value is copied in localVariable 'a'.
	public static void incrementPrimitiveDT(int a) {
		a++;
	}

	// here reference is copied, means 'input' is also pointing to 'arr'.
	public static void incrementReferenceDT(int input[]) {
		for(int i=0;i<input.length;i++) {
			input[i]++;
		}
	}


	public static void main(String[] args) {
		int i=10;
		incrementPrimitiveDT(i); // passByValue
		System.out.println(i); // 10


		int arr[]= {1,2,3,4,5};
		incrementReferenceDT(arr); // passByReference
		System.out.println(Arrays.toString(arr)); // [2, 3, 4, 5, 6]
	}
}
```

10. [**Strings are immutable.**](https://youtu.be/4cEsJtuW4YY)
11. [**== & .equals in String.**](https://youtu.be/i7vYjvJOIiw)
12. [**Wrapper class in java.**](https://youtu.be/nYE_P9FG1g0)
    ## - Object creation and memory allocation in Integer class.

```JAVA
    public static void main(String[] args) {
		// case 1:
				Integer i= new Integer(1);
				Integer j=new Integer(1);
				System.out.println(i==j); // false,  coz == check reference address of i and j, and here 'i' is pointing to 1 (i---> 1) and 'j' is pointing to different 1 (j---> 1)
				System.out.println(i.equals(j)); // true

		// case 2:
				Integer a=new Integer(2);
				Integer b=2;

				System.out.println(a==b); // false
				System.out.println(a.equals(b)); // true

		// case 3:
				Integer x=new Integer(3);
				Integer y=x;

				System.out.println(x==y); // true
				System.out.println(x.equals(y)); // true


		// case 4
				Integer p=128;
				Integer q=128;
				System.out.println(p==q); // false
				System.out.println(p.equals(q)); // true

		// case 5 -128 to 127 is in cached memory so they point to same object without creating it instances.
				Integer s=50;
				Integer t=50;
				System.out.println(s==t); // true
				System.out.println(s.equals(t)); // true
    }
```

13. [**Generics in Java.**](https://youtu.be/XMvznsY02Mk)
14. [**isequals and hashcode in java by codingSimplified.**](https://youtu.be/X2AjBFZfFCY)
    - [**isequals and hashcode in java by AnujBhaiya.**](https://youtu.be/HRHMkQ9fWsM)
15. **% operator in JAVA :** **dividend % divisor** - Here two statement is needed to be taken care :-

	- ## **When Divedend < Divisor then answer is dividend.**
	- ## **When Divedend > Divisor then answer lie in between [0 to divisor-1].**
