# Interview


1.	Reverse the linked list - with 3 / 2 pointers?

2.	Delete current node of the linked list (Hint - Logical deletion)

3.	Explain deadlock to a 5-year-old child.

4.	Hashmap - collision handling and retrieval

5.	Fibonaci series - Loop Vs Recursion

6.	Find nth prime number in optimized way

7.	Sorting - 1 to 100 distinct numbers in O(n)

8.	What is a web application?

9.	What happens when you type google.com in browser.

10.	What do you know about cloud?

11.	REST Service – what will be the HTTP response if there is no data to return? - HTTP 204 No Content

12.	How HTTP 204 No Content differs from 404 Not Found?

13.	Why did you use Spring/Spring boot?

14.	Which loop is faster among following-
	String name = "Shankar";
	for(int i=0; i<10; i++) {
		System.out.println(name);
	}
	for(int i=0; i<10; i++) {
		System.out.println("Shankar");
	}
	Ans: Both will take same time as Java maintains the string literal pool

15.	What does the following program print:
	class Base {
		public String name = "Base";
	}

	class Child extends Base {
		public String name = "Child";
	}

	public class Main {
		public static void main(String[]a) {
			Base b = new Child();
			System.out.println(b.name);
		}	
	}
	Ans: Base

16.	Cut a circular cake in 8 equal sections with only 3 cuts
	- Ans-> Horizontal, Vertical and a cross section cut
	- Tweak in the question - it’s a cream cake, make sure every piece has cream.
	- Ans-> Horizontal, Vertical cuts, then stack the 4 pieces on top of each other, one cut through all the pieces.

User			
User

 ID | Name | Enabled | Salary |
--- | --- | --- | --- |
1   | Vignesh | TRUE | 20000
2   | Bhushan | TRUE | 21000
3   | Anant | FALSE | 21000
4   | Vivek | FALSE | 19500
 
 ROLES

 ID | Name 
--- | --- |
1   | VP | 
2   | MANAGER | 

USER_ROLES

USER_ID | ROLE_ID 
--- | --- |
1   | 2 | 
2   | 1 | 
		


Find out users who do not have any role.

Select user.name, role_id from users
                left outer join user_roles on user.id=user_roles.user_id
Where role_id is null.

Find out user with highest or second highest salary.

Select max(salary_ from users where salary < ( select max(salary) from users)
