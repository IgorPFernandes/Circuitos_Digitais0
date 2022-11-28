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

