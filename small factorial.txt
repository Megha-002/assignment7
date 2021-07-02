import java.util.*;
import java.lang.*;
import java.io.*;
import java.math.BigInteger;
class Codechef
{
   public static void main (String[] args) throws IOException
    {
        final BufferedReader bf = new BufferedReader(new InputStreamReader(System.in));
        final int t = Integer.parseInt(bf.readLine());
        for(int i=0 ;i<t ;i++)
        {
            System.out.println(fact(Integer.parseInt(bf.readLine())));
        }
    }
    private static BigInteger fact(int n)
    {
        BigInteger result = BigInteger.ONE;
        for(int i=2;i<=n;i++)
        {
            result = result.multiply(BigInteger.valueOf(i));
        }
        return result;
    }
}