

<br/>
<img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/cd6c7775-5e18-4cb7-b367-4364af5e81c0" width="80">
&nbsp;&nbsp;&nbsp;&nbsp; <font size ="5"> 2nd Year UBC Integrated Engineering Student - Mechanical & Electrical</font>  

----
### UBC Sailbot - Rudder Mechanical Team Member
[UBC Sailbot Website](https://www.ubcsailbot.org/)
#### Solidworks CAD Parts & Assembly
<img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/18be7fbe-1d6d-4935-bb8d-18311dc1d2e1" width="180"> <img src="https://github.com/ko-vera/ko-vera.github.io/assets/91451073/dcda9d7b-4d81-40f5-aba7-b0ffed2962ce" width="300">

- Structural Stress Calculations
- Integration with Elec team - motors and encoders


### CPEN 312 Labs
#### Lab 1
- logic gates
- Coding in VHDL 
- 8051 Assembly

  
### IGEN 230 Capstone
- use of piezoelectrics
  
<img src="/assets/numpadbreakdown" width="180">
<img src="/assets/numpadexploded" width="180">

![Untitled video - Made with Clipchamp](https://github.com/ko-vera/ko-vera.github.io/assets/91451073/953a51cf-c60d-465f-b170-7065d8c8f2f6)

  
### IGEN 230 Line Following Robot
- using h-bridge, pwm controller
#### Written Arduino Code
<p>'int mr1=6;  //motor left 1
<br>
int mr2=7;  //motor left 2
<br>
int ml1=5;  //motor right 1
<br>
int ml2=4;  //motor right 2'</p>

`const int sens1=A0;   //1st sensor`
`const int sens2=A1;   //2nd sensor`
`const int sens3=A2;   //3rd sensor`

`const int THRESH1 = 1020;`

`int sens1_Val = 0;        // value read from the pot`
`int sens2_Val = 0;`
`int sens3_Val = 0;`

`int output1_Val = 0;     // value output to the PWM (analog out)`
`int output2_Val = 0;`
`int output3_Val = 0;`

`int enr=3;`
`int enl=9;`

`int vspeed=160;`
`int tspeed=140;`
`int stopdelay=30;`
`int godelay=30;`


'void   setup()'
'{'
  'Serial.begin(9600);'

' pinMode(ml1,OUTPUT);'
' pinMode(ml2,OUTPUT);'
' pinMode(mr1,OUTPUT);'
' pinMode(mr2,OUTPUT);'
' pinMode(enr, OUTPUT);'
' pinMode(enl, OUTPUT);'
' pinMode(sens1,INPUT);'
' pinMode(sens2,INPUT);'
 pinMode(sens3,INPUT);
   
}

void loop()
{
 
   sens1_Val=analogRead(sens1);
   sens2_Val=analogRead(sens2);
   sens3_Val=analogRead(sens3);


   // map it to the range of the analog out:
   output1_Val = map(sens1_Val, 0, 1023, 0, 255);
   output2_Val = map(sens2_Val, 0, 1023, 0, 255);
   output3_Val = map(sens3_Val, 0, 1023, 0, 255);


  Serial.print("sensor 1= ");
  Serial.print(sens1_Val);
  Serial.print("\t output 1= ");
  Serial.print(output1_Val);


  Serial.print("\t sensor 2= ");
  Serial.print(sens2_Val);
  Serial.print("\t output 2= ");
  Serial.print(output2_Val);

  Serial.print("\t sensor 3= ");
  Serial.print(sens3_Val);
  Serial.print("\t output 3= ");
  Serial.println(output3_Val);


  // wait 2 milliseconds before the next loop for the analog-to-digital
  // converter to settle after the last reading:
  delay(2);
  

  if(sens3_Val<THRESH1 && sens1_Val<THRESH1)
  {
  backward();
  stopmotor();
  }

  if(sens1_Val>THRESH1 && sens3_Val<THRESH1)
  {
  right();
  stopmotor();
  }
 
  if(sens1_Val<THRESH1 && sens3_Val>THRESH1)
   { 
  left();
  stopmotor();
  }
  
  if(sens1_Val>THRESH1 && sens3_Val>THRESH1)
   {
    delay(godelay);
    stopmotor();
    forward();
  }




}

void forward()
 {
  digitalWrite(mr1,LOW);
  digitalWrite(mr2,HIGH);
  digitalWrite(ml1,LOW);
  digitalWrite(ml2,HIGH);
  analogWrite (enr,vspeed);
  analogWrite (enl,vspeed);
  delay(godelay);
 } 

void backward()
   {
    digitalWrite(mr1,HIGH);
    digitalWrite(mr2,LOW);
    digitalWrite(ml1,HIGH);
    digitalWrite(ml2,LOW);
    analogWrite (enr,vspeed);
    analogWrite (enl,vspeed);
    delay(godelay);
   }

void right()
   {
    digitalWrite(mr1,LOW);
    digitalWrite(mr2,HIGH);
    digitalWrite(ml1,LOW);
    digitalWrite(ml2,HIGH);
    analogWrite (enr,0.5*tspeed);
    analogWrite (enl,tspeed);
    delay(godelay);
   } 

void left()
   {
    digitalWrite(mr1,LOW);
    digitalWrite(mr2,HIGH);
    digitalWrite(ml1,LOW);
    digitalWrite(ml2,HIGH);
    analogWrite (enr,tspeed);
    analogWrite (enl,0.5*tspeed);
    delay(godelay);
   }  

void stopmotor()
 {
  analogWrite (enr,0);
  analogWrite (enl,0);
  delay(stopdelay);

 }


