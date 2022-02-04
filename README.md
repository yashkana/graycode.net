# graycode.net
using System;<br>
<br>
namespace Exercises<br>
{
    class GrayCode<br>
    {
        static int getGray(int n)<br>
        {<br>
            return n ^ (n >> 1);<br>
        }<br>
        static void Main(string[] args)<br>
        {<br>
            int InputNum, GrayNum;<br>
            Console.Write("\nEnter the decimal number:");<br>
            InputNum = Convert.ToInt32(Console.ReadLine());<br>
            Console.Write("\n Binary equivalent of {0} : {1}", InputNum, Convert.ToString(InputNum, 2));<br>
<br>
            GrayNum = getGray(InputNum);<br>
            Console.Write("\n GrayCode equivalent of {0} : {1}", InputNum, Convert.ToString(GrayNum, 2));<br>
        }<br>
    }<br>
}<br>

Output
![Screenshot 2022-02-04 050103](https://user-images.githubusercontent.com/98301023/152474793-7e015e41-838d-40f9-a5c4-96c75a0c2661.png)
