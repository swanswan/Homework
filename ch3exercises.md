Homework 09-20-2014

1. a) T. The source code for a class is usually stored in a separate file, so it makes sense to label the source file with the name of the class.
b) T. All names are case-sensitive and all class names must begin with a capital.
c) F. The import tells the compiler which other classes are used BY this class.
 
4. a) T. The attributes of an object usually aren't used outside of its class.
b) T. An object must be created with the new operator before being initialized.
c) T. A class may have several constructors that differ in number and/or types of parameters.
d) T. Because you can?
e) F. The program calls the new method.
 
5. 1) Even if the fields change, the rest of the project won't be affected.
2) The programmer can document the class for other programmers by describing all constructors and public methods without documenting all implementation methods.
3) It makes maintaining, documenting, and reusing a class easier.
 
7. The first is the column, the second is the row. Rows and columns are counted from 0.
 
11. 
 
package test;
 
public class Book {
	private int numPages;
	private int currentPage;
	
	public void initialize(int page){
		numPages = page;
		currentPage=1;
	}
 
	public int getNumPages() {
		return numPages;
	}
 
 
	public int getCurrentPage() {
		return currentPage;
	}
	
	public void nextPage(){
		if (currentPage < numPages){
			currentPage++;
		}
	}
 
}
 
 
 
package test;
 
public class BookTest {
	
	public static void main(String[] args){
		Book twilight = new Book();
		twilight.initialize(3);
		for(int i=0; i<3; i++){
			System.out.println("The current page is:" + twilight.getCurrentPage());
			twilight.nextPage();
			
		}
	}
}
 
 
14. a) T
b) F
 
16. a, g
