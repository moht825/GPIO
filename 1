//GPIO_Test_Serial.c
#include <stdio.h>
#include <string.h>
#include <wiringPi.h>
#include <wiringSerial.h>

#define GPIO0 0  //Physerial 11
#define GPIO3 3  //Physerial 15

#define baud_rate 115200

int main(void)
{
   
   int fd;
   unsigned char test;
   if(wiringPiSetup() == -1)
   {
      printf("wiringPi Setup error !\n");
      return -1;
   }
   
   if((fd = serialOpen("/dev/ttyACM0", baud_rate))<0)
   {
     printf("UART open error ! \n");
     return -1;
      
   }    
   
   pinMode(GPIO0, INPUT);
   pinMode(GPIO3, INPUT);
   
   printf("GPIO PIN3 : LOW \n");
   digitalWrite(GPIO3, LOW);
   delay(1000);
   
   while(1)
   {
      printf("GPIO0 Pin Read : %1d \n", digitalRead(GPIO0));
      delay(1000);
      /*
      printf("GPIO PIN3 : LOW \n");
      digitalWrite(GPIO3, LOW);
      delay(1000);
      */
   }
   return 0;
}
//Makefile
CC = g++

CFLAGS = -w -Wall -O2
SRCS = GPIO_Test_Serial.c -lwiringPi

PROG = test

OPENCV = `pkg-config --cflags --libs opencv`
LIBS = $(OPENCV)

$(PROG):$(SRCS)
	$(CC) $(CFLAGS) -o $(PROG) $(SRCS) $(LIBS)
	
	$(./PROG)
