#reference
Methods

Wednesday, January 25, 2023

8:13 PM

 

Static Main

<table>
<colgroup>
<col style="width: 8%" />
<col style="width: 91%" />
</colgroup>
<thead>
<tr class="header">
<th><p>    1</p>
<p>    2</p>
<p>    3</p>
<p>    4</p>
<p>    5</p>
<p>    6</p>
<p>    7</p>
<p>    8</p>
<p>    9</p>
<p>   10</p></th>
<th><p>package fibonacci_project;</p>
<p> </p>
<p>public class Fibonacci {</p>
<p>        </p>
<p>        public static void main(String[] args) {</p>
<p>                </p>
<p>                Calculate calculateFib = new Calculate();</p>
<p>                System.out.println(calculateFib.CalculateFibNum(4));</p>
<p>        }</p>
<p>        }</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

Static Int

<table>
<colgroup>
<col style="width: 14%" />
<col style="width: 85%" />
</colgroup>
<thead>
<tr class="header">
<th><p>    1</p>
<p>    2</p>
<p>    3</p>
<p>    4</p>
<p>    5</p>
<p>    6</p>
<p>    7</p>
<p>    8</p>
<p>    9</p>
<p>   10</p>
<p>   11</p>
<p>   12</p>
<p>   13</p>
<p>   14</p>
<p>   15</p>
<p>   16</p>
<p>   17</p></th>
<th><p>package fibonacci_project;</p>
<p> </p>
<p>public class Calculate {</p>
<p> </p>
<p>        static int CalculateFibNum(int n) {</p>
<p>                int num1 = 0;</p>
<p>                int num2 = 1;</p>
<p>                int num3 = 1;</p>
<p>                for (int i = 2; i &lt; n; i++) {</p>
<p>                        num3 = num1 + num2;</p>
<p>                        System.out.println(num3);</p>
<p>                        num1 = num2;</p>
<p>                        num2 = num3;</p>
<p>                }</p>
<p>                return num3;</p>
<p>        }</p>
<p>}</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

 

 

Method Overriding

![[00_Methods_image001.gif]]

Method Overloading

![[00_Methods_image002.gif]]

 

 

 

 

 

 

 

 

 

|     |     |     |     |     |     |
|-----|-----|-----|-----|-----|-----|
|     |     |     |     |     |     |

 
