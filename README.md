# Background

I'm a deadhead. I love the variety of songs that come up at Dead & Company shows, and I love trying to guess what they're going to play next. There are a few intuitive heuristics I use to make my guesses:

* **What did they just play?**
  * There are several fabled sequences of Grateful Dead songs, like "China Cat Sunflower" seguing into "I Know You Rider". Or "Help On The Way" into "Slipknot" into "Franklin's Tower". Knowing these sequences makes it pretty easy to guess what's coming up soon.
* **What set is it?**
  * First and second sets have different feels to them. The first set is usually a bit shorter and features more songs with shorter runtimes. The second set will always have a "Drums > Space" section. Songs tend to be longer and "jammier".
* **What day of the week is it?**
  * Shows on Saturdays will *almost* always feature "One More Saturday Night" at some point
  * Sunday shows usually feature "Samson and Delilah" (and you never want to miss a Sunday show).
* **What did they play yesterday, or the day before?**
  * Go to three or four shows in a row, and it's unlikely you'll hear the same song twice.
* **Where's the show?**
  * Some songs reference specific locations, which confirmation bias tells me means they'll be more likely to be played in (or near) those locations. 

What if there was a way to guess what was going to get played at a show? Does being surprised by the setlist make the show more enjoyable? Is working on a light-hearted project a good way to decompress after a ten-month graduate program? The answer to the last question is probably yes. The others - who knows?

# Predicting Setlists
Predicting setlists is tricky. Ideally we want to incorporate all of the information listed above into making our guesses.

Let's consider the neural network as a potential solution. Neural nets are built with the intent of mimicking the human brain, learning to pick up on patterns and connections that might not be visible to human study.

In this case, we likely want to build something similar to text prediction. Predicting a setlist is actually pretty similar to predicting a sentence. If we treat songs like words, we'll adapt a grammar - certain songs won't appear before or after others - and we'll also be able to predict when a set might end.
