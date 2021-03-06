# Random C Syntax Generator

Randomly generates a syntactically correct C snippet. This short Java program generates C code using a set of production rules. 
<br>

<h4>Instructions for executing the program:</h4>
1. To open the program, double click on the executable file 'exec.jar'.
You need to have the <i>Java Runtime Environment</i> installed on your computer. You can
download it <a href="https://www.java.com/en/download/">here</a>.<br>
2. By clicking on 'Save to File' the randomly generated code is saved into a file named 'random_C.txt'. <br>
3. The source code can be found inside the folder named 'src'.  <br>
4. If you have any problems executing this program, do not hesitate to contact me. <br>

<h4>Production Rules set used to define a subset of the C programming language. </h4>

<pre>
<b><'prog></b> ::= "int main() { <'stat_list> return 0; }"
<br>
<b><'stat_list></b> ::= <'stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | <'stat_list> <'stat>
<br>
<b><'stat></b> ::= <'cmpd_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'if_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'iter_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'assgn_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'decl_stat>
<br>
<b><'cmpd_stat></b> ::= { <'stat_list> }
<br>
<b><'if_stat></b> ::= if ( <'exp> ) <'stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | if ( <'exp> ) <'cmpd_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | if ( <'exp> ) <'stat> else <'stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | if ( <'exp> ) <'cmpd_stat> else <'stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | if ( <'exp> ) <'stat> else <'cmpd_stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | if ( <'exp> ) <'cmpd_stat> else <'cmpd_stat>
<br>
<b><'iter_stat></b> ::= while ( <'exp> ) <'stat>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | while ( <'exp> ) <'cmpd_stat>
<br>
<b><'assgn_stat></b> ::= <'id> = <'exp> ;
<br>
<b><'decl_stat></b> ::= <'type> <'id> ;
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | <'type> <'assgn_stat>
<br>
<b><'exp></b> ::= <'exp> <'op> <'exp>
&nbsp &nbsp &nbsp &nbsp &nbsp | <'id>
&nbsp &nbsp &nbsp &nbsp &nbsp | <'const><'op> ::= + | - | * | /
<br>
<b><'type></b> ::= int
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| double
<br>
<b><'id></b> ::= <'char><'chardigit_seq>
<br>
<b><'const></b> ::= <'digit><'digit_seq>
<br>
<b><'char_digit_seq></b> ::= [empty]
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'char><'char_digit_seq>
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp| <'digit><'char_digit_seq>
<br>
<b><'digit_seq></b> ::= [empty]
&nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp | <'digit><'digit_seq>
<br>
<b><'char></b> ::= [A-Z] | [a-z] | _
<br>
<b><'digit></b> ::= [0-9]
</pre>

<h4>Examples of code generated by my program</h4>
<pre>
int main() {
while (14 - _)
{
c70 = X;
{
if (4757493620) {
_d45_ = B;
}
while (5)
j8__547_Q = 244;
_h = g8;
}
if (45)
while (_ * 28)
_0 = 1;
else b = 4 + G1_7 + 4 * b2;
double c20_1P631_0;
_1 = 1;
}}
return 0;
}
</pre>
<pre>
int main() {
{
if (F)
double K = _;
else
int v_15;
{if (2) {
_ = 4;
}
else jF = 7 + 7;
} }
return 0;
}
</pre>
<pre>
int main() {
if (O) {
if (9374) {
nJ = _b96_;
while (5 / M9 + 9 / 409)
{
double mI;
}
while (2)
_ = U;
} }
else
while (Rsoa)
E = 96 * 4;
return 0; }
</pre>
