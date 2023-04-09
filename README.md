# LexicalAnalysis
词法分析器
## 一个简易的词法分析器
1）处理的语言：类似于PASCAL源程序。
2）输出结果：二元式序列。
3）该语言的单词符号包括：
保留字（10种）：
program  begin  end  var  integer  if  then  else  do  while
标识符
整型常数
界符、运算符（11种）：
＋  －  （  ）  =  >  <
;（分号，语句结束时使用）
,（定义变量时分隔多个变量）
:（冒号，定义变量时使用）
:=（冒号+等号，赋值号）
4）输入方式：文本文件（如：.txt）。
5）输出方式：文本文件（如：.txt）。
每个单词表示成二元组（单词种别，属性值），参见后面输出形式。
6）测试程序样例：
program example;
var k, m, n: integer;
begin
k:=8;
m:=5;
n:=k+m;
if n>10 then
k:=k-1;
end;
7）输出形式：
（1）（1，—）
（2）（11，example）
（3）（4，—）
（4）…
