# Homework3
public class MainClass
{
    String  class_string= "Hello,world" ;

public String gietClassString()
    {
        return this.class_string;
    }
}

import org.junit.Assert;
import org.junit.Test;

public class MainClassTest extends MainClass {
    @Test
    public void testGetClassString() {
        String a = this.gietClassString();
        String s1 = "hello";
        String s2 = "Hello";
        String a1=a.toLowerCase();
        if (a.contains(s2)||a1.contains(s1.toLowerCase()))
        {
            Assert.assertTrue("there is not a single substring Hello or hello",a1.contains(s1.toLowerCase())==a.contains(s2)==true);
        }


        }


}

 
