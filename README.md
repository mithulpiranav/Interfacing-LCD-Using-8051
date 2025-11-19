# Interfacing-LCD-Using-8051

## Aim:
To interface a 16x2 LCD with an 8051 microcontroller and display your name.

## Apparatus Required:
•	Laptop with Keil uVision software
•	Proteus Design Suite

## Algorithm:
1.Configure LCD in 4-bit mode.
2.Initialize LCD with commands.
3.Move the cursor direction.
4.Display ON
5.Set cursor position to the beginning (optional).
6.Send each character of the string "NAME" to the LCD one by one using data mode.
7.Continuously run the program to keep displaying the message.

## Program :
```
#include<reg51.h>
void main()
{
unsigned char x,y;
unsigned int i;
P1=0x00;
while(1)
	{   
	x=0x01;
	for(y=0;y<8;y++)	
		{
		P1=x;
    for(i=0;i<60000;i++);
    x=x<<1;
    }			
	}	
}
```


## Output :
<img width="1236" height="716" alt="image" src="https://github.com/user-attachments/assets/7ad2818c-bcc7-43e8-ac67-e95965281fd4" />


## Result :  
Thus interfacing LCD using 8051 microcontroller is executed successfully.

