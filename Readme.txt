###   TEMPLATE

{"NAME":"LSC-RGBW-Strip","GPIO":[51,0,0,0,37,0,0,0,38,40,39,0,0],"FLAG":0,"BASE":18}4


###   komendy które wklejamy w konsoli:

rule1 on IrReceived#Data=0x00F7C03F do power1 on endon on IrReceived#Data=0x00F740BF do power1 off endon on IrReceived#Data=0x00F700FF do dimmer + endon on IrReceived#Data=0x00F7807F do dimmer - endon on IrReceived#Data=0x00F7D02F do scheme 0 endon on IrReceived#Data=0x00F7F00F do scheme 4 endon on IrReceived#Data=0x00F7C837 do scheme 2 endon on IrReceived#Data=0x00F7E817 do scheme 3 endon 

rule2 on IrReceived#Data=0x00F720DF do color2 #FF000000 endon on IrReceived#Data=0x00F710EF do color2 #470D0000 endon on IrReceived#Data=0x00F730CF do color2 #38160000 endon on IrReceived#Data=0x00F708F7 do color2 #331E0000 endon on IrReceived#Data=0x00F728D7 do color2 #33280000 endon on IrReceived#Data=0x00F7A05F do color2 #00FF0000 endon on IrReceived#Data=0x00F7906F do color2 #00330A00 endon on IrReceived#Data=0x00F7B04F do color2 #00331400 endon on IrReceived#Data=0x00F78877 do color2 #00331E00 endon

rule3 on IrReceived#Data=0x00F7A857 do color2 #00332800 endon on IrReceived#Data=0x00F7609F do color2 #0000FF00 endon on IrReceived#Data=0x00F750AF do color2 #0A003300 endon on IrReceived#Data=0x00F7708F do color2 #14003300 endon on IrReceived#Data=0x00F748B7 do color2 #14003300 endon on IrReceived#Data=0x00F76897 do color2 #28003300 endon on IrReceived#Data=0x00F7E01F do color2 #000000FF endon

Backlog rule1 1; rule2 1; rule3 1
