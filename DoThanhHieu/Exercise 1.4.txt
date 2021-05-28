Ex1.4
a, Write a Java:
import java.util.Vector;

class Vector 
{
	public static Vector union(Vector a, Vector b)
	{
		Vector v = new Vector();
		v.addAll(a);
		v.addAll(b);
		
	}
}

class Vectortest  
{
	public static void main(String[] arg)
	{
		Vector a = new Vector();
		a.add(2);
		Vector b = new Vector();
		b.add(3);
		Vector v = union(a, b);
  	}
}

b, We need to write a method checking value of variables is not null.
c, 
class Vectortest  
{
	public static void main(String[] arg)
	{
		Vector a = new Vector();		
		Vector b = new Vector();
		b.add(3);
		Vector v = union(a, b);
  	}
}
d, 
class Vector 
{
	public static Vector union(Vector a, Vector b)
	{
		if (a.isEmpty()  && b.isEmpty())
		{
			System.out.printf("error!, vector a and vector b is not null");
			
  		else
		{
			Vector v = new Vector();
			v.addAll(a);
			v.addAll(b);
		}
	}
}
