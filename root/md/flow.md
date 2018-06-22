### 这是flow示例的页面

## 图1

``` flow
st=>start: Start:>http://www.google.com[blank]
e=>end:>http://www.google.com
op1=>operation: My Operation
op2=>operation: 'Stuff'|current
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No? :>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|request
st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(true)->io->e
c2(false)->op2->e
```

## 图2

``` flow
st=>start: Start:>http://www.google.com[blank]
e=>end:>http://www.google.com
op1=>operation: My Operation
op2=>operation: 'Stuff'|current
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No? :>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|request
st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(true)->io->e
c2(false)->op2->e
```
