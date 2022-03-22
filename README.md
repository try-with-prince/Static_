public class Learn {
    static  int a = 10;
    Learn(){
System.out.println("dfsf");
    }
     static void d()
    {
        System.out.println(a+300);
    }

    public static void main(String[] args) {
        System.out.println(a);//static varriable store in method area with static method so no neccesary to call with ob.
        Learn a1 = new Learn();

        a1.a=90;
        //static varriable ki value change karne per orignal value change hoti h bcz static varriable orignal
        //value share karta h
        System.out.println(a1.a);
        Learn a2= new Learn();
        //a2.a=30;

        d();
        {
            System.out.println("bdvbdbv");
        }

        //a = a + 20;
        System.out.println(a);
        a2.a=70;
        System.out.println(a2.a);
        System.out.println(a);
        Learn f2=new Learn();
        f2.d();{
            System.out.println("ff");
        }
    }
        //System.out.println("dsnjn");
    static{
        System.out.println(a=100);
    }
        /*public static void m1()
        {
            System.out.println(a);
        }
    }
*/
    /*static void  m1() {
         System.out.println(a1.a);
    }
*/

    {
        System.out.println("jvfd");
    }
}
/*
100
100
jvfd
dfsf
90
jvfd
dfsf
390
bdvbdbv
90
70
70
jvfd
dfsf
370
ff

Process finished with exit code 0
*/
