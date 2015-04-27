memory(m)
Prgm
©NUMBER
FnOff 1,2,3,4,5
If m>12 Then
  Text "Number too large"
  Stop
EndIf
If m<1 Then
  Text "Number too small"
  Stop
EndIf
int(m)­→n
Lbl a
ClrIO
ClrDraw
ClrGraph
setGraph("Coordinates","OFF")
setGraph("Grid","OFF")
setGraph("Axes","OFF")
int(rand()*10^n)­→x
While x≤10^(n-1)
  int(rand()*10^n)­→x
EndWhile
int(rand()*50)­→z
rand(3)-2­→a
rand(3)-2­→b
0­→c
rand(56)+10­→d
rand(95-5*(n-8))+5­→e
PxlText string(x),d,e
PxlHorz 76
0­→p
For y,0,50
  getKey()­→k
  If k=13 Then
    Exit
  EndIf
  PxlOff 76,p
  p+1­→p
  PxlOff 76,p
  p+1­→p
  PxlOff 76,p
  p+1­→p
  If mod(y,10)=0 Then
    PxlOff 76,p
    p+1­→p
  EndIf
  If c=z Then
    int(rand()*50)­→z
    0­→c
    rand(3)-2­→a
    rand(3)-2­→b
  EndIf
  c+1­→c
  d+a­→d
  If d<10 Then
    10­→d
    z­→c
  EndIf
  If d>60 Then
    60­→d
    z­→c
  EndIf
  e+b­→e
  If e<5 Then
    5­→e
    z­→c
  EndIf
  If e>95-5*(n-8)+5 Then
    95-5*(n-8)+5­→e
    z­→c
  EndIf
  PxlText "              ",d-8,e-4
  PxlText " "&string(x)&" ",d,e-4
  PxlText "              ",d+8,e-4
EndFor
ClrDraw
Input "What is the number?",y
If x=y Then
  Disp "Good Job!"
Else
  Disp "Sorry! The number was",string(x)
EndIf
Input "Again? (0=no 1=yes)",x
If x=1 Then
  Goto a
Else
  DispHome
EndIf
EndPrgm
