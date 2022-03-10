# salary
import java.util.*;
class employe
{
    String name;
    int id,salary,hours;
    Scanner k =new Scanner(System.in);
    void getinfo()
    {
        System.out.println("enter name of employ");
        name=k.nextLine();
        System.out.println("enter id of employ");
        id=k.nextInt();
        System.out.println("enter salary of employ");
        salary=k.nextInt();
        System.out.println("enter hours of employ");
        hours=k.nextInt();
    }
    void addsal()
    {
        if(salary<500)
        {
        salary=salary+10;
        }
    }
    int addwork()
    {
        if(hours>6)
        {
            salary=salary+5;
        }
        else
        {
            salary=salary;
        }
        return salary;
    }
}
class Main
{
    public static void main(String[]args)
    {
        Scanner s=new Scanner(System.in);
        System.out.println("enter n of employ");
        int n=s.nextInt();
        int i;
        employe o[]=new employe[n];
        for(i=0;i<=n;i++)
        {
        o[i]=new employe();
        o[i].getinfo();
        o[i].addsal();
        System.out.println("o[i].addwork()");
    }
}
}

