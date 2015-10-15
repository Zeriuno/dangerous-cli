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
mv,cp,rm
2.3.1
$ echo "hello, world" > foo.txt
$ cp foo.txt bar.txt
$ diff foo.txt bar.txt
2.3.2
$ cat foo.txt > baz.txt
2.3.3
$ cat foo.txt bar.txt > quux.txt
4. rm -f doesn't return the error message

2.4
2.4.1
$ echo "FRom faireſt creatures we deſire increaſe,
 That thereby beauties Roſe might neuer die,
 But as the riper ſhould by time deceaſe,
 His tender heire might beare his memory:
 But thou contracted to thine owne bright eyes,
 Feed’ſt thy lights flame with ſelfe ſubſtantiall fewell,
 Making a famine where aboundance lies,
 Thy ſelfe thy foe,to thy ſweet ſelfe too cruell:
 Thou that art now the worlds freſh ornament,
 And only herauld to the gaudy ſpring,
 Within thine owne bud burieſt thy content,
 And tender chorle makſt waſt in niggarding:
    Pitty the world,or elſe this glutton be,
    To eate the worlds due,by the graue and thee." > sonnet_1_complete.txt
2.4.2
$ touch foo
$ move foo bar
$ cp bar baz
2.4.3
$ ls b*
2.4.4
$ rm ba*

3.1
$ echo foo
foo
$ ls
[...]
$ !!
ls
[...]
$ !echo
echo foo
foo
3.1.1
$ curl -I www.learnenough.com
HTTP/1.1 200 OK
Date: Sat, 10 Oct 2015 13:28:18 GMT
Content-Type: text/html; charset=utf-8
Connection: keep-alive
Set-Cookie: __cfduid=dc49abef1bf6c50a2379ba290a48eaf341444483697; expires=Sun, 09-Oct-16 13:28:17 GMT; path=/; domain=.learnenough.com; HttpOnly
Status: 200 OK
X-Frame-Options: SAMEORIGIN
X-Xss-Protection: 1; mode=block
X-Content-Type-Options: nosniff
Etag: W/"af0958373195e283b4ec8ca69a407e1a"
Cache-Control: max-age=0, private, must-revalidate
X-Request-Id: 04d630df-46f7-4c37-8953-ea05d223fd2e
X-Runtime: 0.249633
Via: 1.1 vegur
Server: cloudflare-nginx
CF-RAY: 2332aae6d3de08fc-CDG

3.1.2
$ ls -rtl
sonnets is 95635
3.1.3
$ ls -hl
3.1.4
$ ls -hartl

3.2
$ head sonnets.txt
[...]
$ tail !$
[...]
$ wc sonnets.txt
$ head !$ | wc
#When piping to wc, the file name isn't showed in the output.
| works when the program can take stdin as input
3.2.1
$ tail sonnets.txt | wc
$ man head
$ head -n 1 sonnets.txt
$ head -n 2620 sonnets.txt
$ tail -n 20 sonnets.txt
$ tail -n 2620 sonnets.txt
3.2.2
$ head -n 18 sonnets.txt
3.2.3
$ head -n 18 sonnets.txt | tail -n 14
3.2.4
$ tail -f learnenough

3.3.1
$ less sonnets.txt
ctrl F / Space
ctrl B
g -> go to beginning
<NUMBER>G go to line <NUMBER>
$ less -N sonnets.txt
-> less shows line numbers.

3.3.2
/All[return]
n
[...]
N
[...]
-10-
3.3.3
$ less sonnets.txt
/Let me not[return]
n
3.3.4
$ man ls
/sort
$ ls -rS

3.4
$ man grep
/case
$ grep -i rose sonnets.txt | wc
$ ps aux
$ ps aux | grep flash
$ kill -9 $pid
$ kill -9 -f $name
3.4.1
$ man grep
/line number
n
$ grep -n rose sonnets.txt
$ grep -ni rose sonnets.txt
3.4.2
$ grep -ni rose sonnets.txt
$ less sonnets.txt
2203G
3.4.3
$ grep -ni rose sonnets.txt | head -n 1
3.4.4
$ grep Rose sonnets.txt | wc
-> 3 lines

3.5.1
$ history | less
-> ls
$ history | wc
1026
