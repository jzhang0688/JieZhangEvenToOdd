# JieZhangEvenToOdd

package com.company;

public class Main{

    public static void main(String[] args)
    {
        System.out.println(EvenToOdd("Hello"));
    }

    public static String EvenToOdd(String str)
    {
        int i = 0;
        int oi=1;
        String odd = "";
        String even = "";
        while (i < str.length())
        {
            even = even + str.substring(i,i+1);
            i=i+2;
        }
        while(oi < str.length())
        {
            odd = odd + str.substring(oi,oi+1);
            oi = oi+2;
        }
        return even + odd;
    }
}
