abstract class RBIBank{
    public abstract int getRateOfInterest();
}
class SBI extends RBIBank{
    public int getRateOfInterest(){
        return 7;
  }
}
class UB extends RBIBank{
    public int getRateOfInterest(){
        return 8;
    }
}
public class Bank{
    public static void main (String[] args) {
    RBIBank s=new SBI();
    RBIBank p=new UB();
    System.out.println("Rate of Interest in SBI is: "+s.getRateOfInterest()+" %");
    System.out.println("Rate of Interest in UB is: "+p.getRateOfInterest()+" %");
  }
}

