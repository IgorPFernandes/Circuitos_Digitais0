# Circuitos_Digitais0

<br>

##Exercício 1:
=
%%file exercicio.sv

/*

Módulo exercicio

*/
module exercicio(a,b,cin,cout,s);
  input a,b,cin;
  output cout,s;

  assign s = (a ^ b) ^ cin;
  assign cout = (a & b) | (b & c) | (a & c);

endmodule

##Exercício 2:
=

%%file exercicio.sv

/*

Módulo exercicio

*/
module exercicio( a, b, c, z );
  // Declaração de portas
  input a, b, c;
  output z;

  // Fluxo de dados
  assign z = (b & ~a) | (a | ~c) | (~b & c);

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
  input a,b;
  output s;

  assign s = (a + b);

endmodule

##Exercício 6:
=


