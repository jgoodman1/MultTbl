# MultTbl

/**
 * Write a description of class MultTable here.
 * 
 * @author (Joshua Goodman) 
 * @version (a version number or a date)
 */
public class MultTable
{
public static void main (String[] args)
{
    System.out.print("   |");
    for (int i = 1; i <=12; i++)
    System.out.print(pad(i) + " ");
    System.out.println();
    System.out.print("---+");
    for (int i = 1; i <= 12; i++)
       System.out.print("---+");
      for (int i = 1; i <= 12; i++)
         System.out.print("-----");
      System.out.println();
      for (int i = 1; i <= 12; i++) {
         System.out.print(pad(i) + "|");
         for (int j = 1; j <= 12; j++) {
            System.out.print(pad(i*j) + " ");
         }
         System.out.println();
      }
   } 
   public static String pad(int x) {
      String s = new String();
      if (x < 10) s = "  " + x;
      else if (x < 100) s = " " + x;
      else s = "" + x;
      return s;
   }
}

