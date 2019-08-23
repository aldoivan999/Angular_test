node {
s t a g e ( ’ Checkout ’ ) {
c h e c k o u t scm
}
stage ( ’ Build ’ ) {
d o c k e r . image ( ’ t r i o n / ng−c l i ’ ) . i n s i d e {
s h ’ npm i n s t a l l ’
s h ’ ng b u i l d −−p r o g r e s s f a l s e −−p r o d −−aot ’
s h ’ t a r −c v z f d i s t . t a r . gz −−s t r i p −components=1 d i s t ’
}
a r c h i v e ’ d i s t . t a r . gz ’
}
s t a g e ( ’ Test ’ ) {
d o c k e r . image ( ’ t r i o n / ng−c l i −karma ’ ) . i n s i d e {
s h ’ ng t e s t −−p r o g r e s s f a l s e −−watch f a l s e ’
}
}
}
