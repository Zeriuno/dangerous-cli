$ echo hello
hello
$ echo 'goodbye'
goodbye
$ echo "goodbye"
goodbye
$ echo hello, goodbye
hello, goodbye
$ echo "hello, goodbye"
hello, goodbye
$ echo "hello, goodbye'
>
>"
$ echo '"hello, goodbye"'
"hello, goodbye"
$ echo 'hello, goodbye
> ^C
$ 

1.3.2
$ echo -n hello

1.4.1

$ echo fee
fee

Upper arrow, back one

$ echo fie
Upper arro
$ echo foe
$ echo fum

1.5-1
$ clear
1.5.2

ctrl Maiuscola T
$ echo 'hello'
hello
$ exit

1.6.1
$ echo '"man echo"'
"man echo"
1.6.2
$ sleep 5
$ sleep 5000
ctrl C
$ sleep 5 && echo "Back on!"
Back on!


2.1

$ echo "From fairest creatures we desire increase" > sonnet_1.txt
$ echo "That thereby beuty's Rose might never die," >> sonnet_1.txt

$ echo "From faires creatures we desire increase" > sonnet_1_lower_case.txt
$ echo "That thereby beauty's rose might never die," >> sonnet_1_lower_case.txt

$ diff sonnet_1.txt sonnet_1_lower_case.txt


2.1.1

$ echo "From faires creatures we desire increase" > line_1.txt
$ echo "That thereby beauty's rose might never die," >> line_2.txt


2.1.2

$ cat line_1.txt > line_1_2.txt
$ cat line_2.txt >> line_1_2.txt
$ diff line_1_2.txt sonnet_1_lower_case.txt


2.1.3

$ cat line_2.txt line_1.txt > sonnet_1_reversed.txt


2.2
$ ls -rtl
#reversed time of modification long form
$ echo "*.txt" > .gitignore

2.2.1
$ ls s*
2.2.2
$ ls -rtl *onnet*
2.2.3
$ ls -artl


2.3
