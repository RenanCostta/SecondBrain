
**Data:** 2025-02-11
**keyboards:** 
**links internos:** 
___

//Código exemplo: 

1. public class SwitchMonthExample {    
2. public static void main(String[] args) {    
3.     //Specifying month number  
4.     int month=7;    
5.     String monthString="";  
6.     //Switch statement  
7.     switch(month){    
8.     //case statements within the switch block  
9.     case 1: monthString="1 - January";  
10.     break;    
11.     case 2: monthString="2 - February";  
12.     break;    
13.     case 3: monthString="3 - March";  
14.     break;    
15.     case 4: monthString="4 - April";  
16.     break;    
17.     case 5: monthString="5 - May";  
18.     break;    
19.     case 6: monthString="6 - June";  
20.     break;    
21.     case 7: monthString="7 - July";  
22.     break;    
23.     case 8: monthString="8 - August";  
24.     break;    
25.     case 9: monthString="9 - September";  
26.     break;    
27.     case 10: monthString="10 - October";  
28.     break;    
29.     case 11: monthString="11 - November";  
30.     break;    
31.     case 12: monthString="12 - December";  
32.     break;    
33.     default:System.out.println("Invalid Month!");    
34.     }    
35.     //Printing month of the given number  
36.     System.out.println(monthString);  
37. }    
38. }