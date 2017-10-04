Hi.  Thank you for taking the time to review my project.

I look forward to your feedback.

Please find my project on the following github site:

https://github.com/netlogic/tv-script-generation-project/commits/master

All work has been committed as it was built.

The lesson on creating the EC2 gpu instance was very helpful.

This made this project so much faster to train than on my 8 core macbook pro (amazing).

My model has a dropout wrapper as per the sentiment project we learned in class
but keep_prob was changed to 1 as .5 did not sure more improvement.  
Perhaps with a larger amount of data other results would be seen.

For token_lookup I decided to use short abbreviations to save on processing time of tokens.

Seems a higher character sequence gets training loss to lower quicker.
Seems for weights initializer using stddev=.1 get us to to a loss quicker than using xavier.

For my hyper params the following combos were tried once I saw the benefit of 32 character sequence.

I decided to stay with the final hyper params below in the list
in my python notebook as the results were satisfactory to meet the rubric of under 1.0

- SeqRate 32 gets us to  0.078 at 75 epochs (256 rnn) LSTM layers = 1  embed_dim = 300
- SeqRate 32 gets us to  0.076 at 75 epochs (512 rnn) so not much advantage LSTM layers = 1  embed_dim = 300
- SeqRate 32 gets us to .091 at 75 epochs (256 rnn) LSTM layers = 2  embed_dim = 300
- SeqRate 32 gets us to .0.073 at 200 epochs (256 rnn) LSTM layers = 2  embed_dim = 300
- SeqRate 32 gets us to .077 at 200 epochs (256 rnn) layers =1 embed_dim = 300
- 32 gets us to .076 at 100 epochs (256 rnn) layers =1 embed_dim = 300


My first script!!!

moe_szyslak: everybody reach in and draw a pickled egg. whoever gets the black egg stays sober tonight.
barney_gumble: noooooooooo!
homer_simpson:(to barney) you got the black egg stays sober tonight.
barney_gumble: now, i thought they was the tough kid. smelly. my shtick was looking into his house from 1895. and that means someone buyin'!
carl_carlson:(sings) full-blooded...
barney_gumble:(off a stool) yeah.
moe_szyslak: you got that straight, barn.
barney_gumble:(sings) my-y-y-y-y-y adeleine.
barney_gumble:(sings) my-y-y-y-y-y adeleine.
barney_gumble:(a roll) we-we-we switch clothes with them, i'm missing the guy.
moe_szyslak:(almost there) that's pretty dumb... but uh...
homer_simpson: extended it!"! that stuff killed my grandmother!
moe_szyslak: so sad.


singers: don't got no candy, i only serve beer, and who said that you take any more.
carl_carlson:(teenage girl) ohmygod, ohmygod, ohmygod....


