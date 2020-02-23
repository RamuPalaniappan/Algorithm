import java.util.Arrays;
public class Main
{
  public static void main (String[]args)
  {
    int[] array = { 52, 42, 72, 32, 47, 87 };
    int n = array.length;
    for (int i = 0; i <= n - 1; i++)
      {
	for (int j = 0; j < n - 1; j++)
	  {
	    if (array[j] > array[j + 1])
	      {
		continue;
	      }
	    else
	      {
		int temp = array[j];
		array[j] = array[j + 1];
		array[j + 1] = temp;
	      }
	  }
      }
    System.out.println (Arrays.toString (array));
  }
}



