1. The two stages are compilation, then execution.
2. The first stage of execution is what defines everything that will be used in the code. So in this case, lines 3, 5, 6, and 8 are all compilation. They are creating a variable and assigning it to a certain context. Global, for 3 and 5, creating foo and bar() within the global scope. Inside bar() for lines 6 and 8.
3. The second stage of execution is the actual execution stage. This is when the actual instructions given to the cpu are executed. The first thing happening on this stage is the computer deciding to execute bar(). Right after that, it executes baz(). Then it redefines the bar scope foo's content to be 'bam'.
4. 3 scopes, global, bar() and baz().
foo: global scope
foo: bar()
bar(): global scope
baz(): bar()
5. It will be assigned to the foo in bar() scope, since that foo is in the same scope as the function invocation. I'm not sure if that's why, but I get that feelings.

6. It won't, it's never declared, simply called.

7. 
16: undefined
17: 'bar'
18: undefined
19: undefined