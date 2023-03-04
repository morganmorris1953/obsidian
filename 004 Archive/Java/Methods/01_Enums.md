Enums

Wednesday, January 25, 2023

8:28 PM

 

|     |     |     |     |
|-----|-----|-----|-----|

Enums

An enum is a special \"class\" that represents a group of constants (unchangeable variables, like final variables).  Enum is short for \"enumerations\", which means \"specifically listed\".

 

**Difference between Enums and Classes**

An enum can, just like a class, have attributes and methods. The only difference is that enum constants are public, static and final (unchangeable - cannot be overridden).

 

An enum cannot be used to create objects, and it cannot extend other classes (but it can implement interfaces).

 

**Why And When To Use Enums?**

Use enums when you have values that you know aren\'t going to change, like month days, days, colors, deck of cards, etc.

 

 

To create an enum, use the enum keyword (instead of class or interface), and separate the constants with a comma. Note that they should be in uppercase letters:

 

<table>
<colgroup>
<col style="width: 39%" />
<col style="width: 60%" />
</colgroup>
<thead>
<tr class="header">
<th><p>    1</p>
<p>    2</p>
<p>    3</p>
<p>    4</p>
<p>    5</p></th>
<th><p>enum Level {</p>
<p>  LOW,</p>
<p>  MEDIUM,</p>
<p>  HIGH</p>
<p>}</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

 

You can access enum constants with the dot syntax:

|     1 | Level myVar = Level.MEDIUM; |
|-------|-----------------------------|

 

Enum inside a Class

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 83%" />
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
<p>   12</p></th>
<th><p>public class Main {</p>
<p>  enum Level {</p>
<p>    LOW,</p>
<p>    MEDIUM,</p>
<p>    HIGH</p>
<p>  }</p>
<p> </p>
<p>  public static void main(String[] args) {</p>
<p>    Level myVar = Level.MEDIUM;</p>
<p>    System.out.println(myVar);</p>
<p>  }</p>
<p>}</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

The output will be:

 

MEDIUM

 

 

 

Enum in a Switch Statement

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 83%" />
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
<p>   17</p>
<p>   18</p>
<p>   19</p>
<p>   20</p>
<p>   21</p>
<p>   22</p>
<p>   23</p></th>
<th><p>enum Level {</p>
<p>  LOW,</p>
<p>  MEDIUM,</p>
<p>  HIGH</p>
<p>}</p>
<p> </p>
<p>public class Main {</p>
<p>  public static void main(String[] args) {</p>
<p>    Level myVar = Level.MEDIUM;</p>
<p> </p>
<p>    switch(myVar) {</p>
<p>      case LOW:</p>
<p>        System.out.println("Low level");</p>
<p>        break;</p>
<p>      case MEDIUM:</p>
<p>         System.out.println("Medium level");</p>
<p>        break;</p>
<p>      case HIGH:</p>
<p>        System.out.println("High level");</p>
<p>        break;</p>
<p>    }</p>
<p>  }</p>
<p>}</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

The output will be:

 

Medium level

 

 

 

Loop Through an Enum

The enum type has a values() method, which returns an array of all enum constants. This method is useful when you want to loop through the constants of an enum:

 

Example

<table>
<colgroup>
<col style="width: 19%" />
<col style="width: 80%" />
</colgroup>
<thead>
<tr class="header">
<th><p>    1</p>
<p>    2</p>
<p>    3</p></th>
<th><p>for (Level myVar : Level.values()) {</p>
<p>  System.out.println(myVar);</p>
<p>}</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

The output will be:

 

LOW

MEDIUM

HIGH

 

 
