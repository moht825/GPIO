//GPIO_Test_Serial_Arduino.c
#include <stdio.h>
#include <string.h>
#include <wiringPi.h>
#include <wiringSerial.h>
#include <termio.h>

#define GPIO0 0  //Physerial 11
#define GPIO3 3  //Physerial 15

#define baud_rate 115200

int getch(void)
{
   
   int ch ;
   struct termios buf;
   struct termios save;
   
   tcgetattr(0, &save);
   buf = save;
   buf.c_lflag &= ~(ICANON|ECHO);
   buf.c_cc[VMIN]=1;
   buf.c_cc[VTIME]=0;
   tcsetattr(0, TCSAFLUSH, &buf);
   ch = getchar();
   tcsetattr(0,TCSAFLUSH, &save);
   return ch;
}
int main(void)
{
   
   int fd;
   unsigned char test,receive_char;
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
   pinMode(GPIO3, OUTPUT);
   
   //printf("GPIO PIN3 : LOW \n");
   //digitalWrite(GPIO3, LOW);
   //delay(1000);
   test = 'B';
   
   while(1)
   {
      test = getch();
      
      if(test == 'A')
      {
         printf(" Input A : %c \n", test);
         serialPutchar(fd,test);
      }
      else
      {
         printf(" Input not A : %c \n", test);
         serialPutchar(fd,test);
      }
      
      delay(50);
      
      while(serialDataAvail(fd))
      {
         receive_char = serialGetchar(fd);
         printf(" Reeceived char : %d %c \n", receive_char, receive_char);
      }
      
      delay(2);
     
   }
   return 0;
}
//Makefile
CC = g++

CFLAGS = -w -Wall -O2
SRCS = GPIO_Test_Serial_Arduino.c -lwiringPi

PROG = test

OPENCV = `pkg-config --cflags --libs opencv`
LIBS = $(OPENCV)

$(PROG):$(SRCS)
	$(CC) $(CFLAGS) -o $(PROG) $(SRCS) $(LIBS)
	
	$(./PROG)
//Serial_test.ino
void setup()
{
  Serial.begin(115200);
}

void loop()
{
  char test = 'A';
  int i;

  if( Serial.available() )
  {
    char a;
    a = Serial.read();
    if(a == 'A') 
    {
      Serial.print("test : A");
    }
    else
    {
      Serial.print("test : not A");
    }
  }
 
    
   
    
  /*
  for(i=0;i<16;i++)
  {
    test = test + 1;

  
  Serial.print(test);
  delay(500);
  }
*/  
}
