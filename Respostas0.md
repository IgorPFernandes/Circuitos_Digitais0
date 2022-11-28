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

/*

Módulo exercicio

*/
module exercicio(izero,a,ione,q);
  input ione,izero,a;
  output q;

  assign q = ((a~&a) ~& ione) ~& (a~&izero)); 

endmodule

##Exercício 4:
=
%%file exercicio.sv

/*

Módulo exercicio

*/
module exercicio(a,b,c,d,e);
  input a,b;
  output c,d,e;

  assign c = (~a&b);
  assign d = (~a&b)~|(a&~b);
  assign e = (a&~b);

endmodule

##Exercício 5:
=

%%file exercicio.sv

/*

Módulo exercicio

*/
module exercicio(a,b,s);
  input [3:0] a,b;
  output [3:0] s;

  assign s = (a + b);

endmodule

##Exercício 6:
=

%%file exercicio.sv

/*

Módulo exercicio

*/
module exercicio(a,b,c,d,e);
  input [3:0] a,b;
  output [3:0] c,d,e;

  assign c = a > b;
  assign d = a = b;
  assign e = a < b;

endmodule

##Exercício 7:
=


