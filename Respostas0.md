# Circuitos_Digitais0

<br>

##Exercício 1:
=
%%file exercicio.sv
<br>
module exercicio(a,b,cin,cout,s);
<br>
  input a,b,cin;
  <br>
  output cout,s;

  assign s = (a ^ b) ^ cin;
  <br>
  assign cout = (a & b) | (b & c) | (a & c);

endmodule

##Exercício 2:
=

%%file exercicio.sv
<br>
module exercicio( a, b, c, z );
<br>
  input a, b, c;
  <br>
  output z;
  <br>
  assign z = (b & ~a) | (a | ~c) | (~b & c);
<br>
endmodule

##Exercício 3:
=

%%file exercicio.sv
<br>
module exercicio(izero,a,ione,q);
<br>
  input ione,izero,a;
  <br>
  output q;
  <br>

  assign q = ((a~&a) ~& ione) ~& (a~&izero)); 
  <br>

endmodule

##Exercício 4:
=
%%file exercicio.sv
<br>
module exercicio(a,b,c,d,e);
<br>
  input a,b;
  <br>
  output c,d,e;
  <br>

  assign c = (~a&b);
  <br>
  assign d = (~a&b)~|(a&~b);
  <br>
  assign e = (a&~b);
  <br>

endmodule

##Exercício 5:
=

%%file exercicio.sv
<br>
module exercicio(a,b,s);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] s;
  <br>

  assign s = (a + b);
  <br>

endmodule

##Exercício 6:
=

%%file exercicio.sv
<br>
module exercicio(a,b,c,d,e);
<br>
  input [3:0] a,b;
  <br>
  output [3:0] c,d,e;
  <br>

  assign c = a > b;
  <br>
  assign d = a = b;
  <br>
  assign e = a < b;
  <br>

endmodule

##Exercício 7:
=

%%file exercicio.sv

<br>
module exercicio(a,b,sel,y);
<br>
  intput a,b,sel;
  <br>
  output y;
  <br>

  assign y = sel ? a:b;
  <br>

endmodule

