Exercise 3.3: JUnit tests
 
public void testEnQueue() 
{
    Object a = 1;
    BoundedQueue instance = new BoundedQueue(2);
    instance.enQueue(a); 
    Assert.assertEquals(instance.toString(), "[1]");
}



public void testDeQueue() 
{       
    Object a = 1;
    Object b = 4;
    BoundedQueue instance = new BoundedQueue(2);
    instance.enQueue(a);
    instance.enQueue(b);
    instance.deQueue();    
    Assert.assertEquals(instance.toString(), "[2]");
}


   
public void testIsEmpty()
{        
    BoundedQueue instance = new BoundedQueue(2);
    assertEquals(instance.isEmpty(), true);
}


	
public void testIsFull() 
{  
   Object a = 1;
   BoundedQueue instance = new BoundedQueue(2);
   instance.enQueue(a);
   instance.enQueue(a);
   assertEquals(instance.isFull(), true);
}

   
public void testToString()
{    
   Object a = 3;
   Object b = 4;
   Object c = 1;
   BoundedQueue instance = new BoundedQueue(3);
   instance.enQueue(a);
   instance.enQueue(b);
   instance.enQueue(c);
   Assert.assertEquals(instance.toString(), "[3, 4, 5]");
}
