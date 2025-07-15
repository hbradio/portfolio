---
title: "Fighting Brandolini's Law with Sampling"
date: "2025-07-08"
---

*[Brady Hurlburt](/) - July 8, 2025*

## "But Don't All Politicians Lie?"

In 2015, Angi Drobnic Holan published [a wonderful article titled "All Politicians Lie. Some Lie More Than Others."](https://www.nytimes.com/2015/12/13/opinion/campaign-stops/all-politicians-lie-some-lie-more-than-others.html)
In it, she makes the case that while all politicians lie, there are meaningful differences in how often and how severely they do so.

Here is the graphic from her piece:

{{< figure src="/media/fact-checking/nyt.png" alt="Holan's analysis of PolitiFact lyting rates from her NYT article" caption="" class="big" >}}

Her article resonates with me because indifference to political dishonesty is surprisingly common in my circle.
In conversations with my peers, when I call out a politician's lie, I'm sometimes met with **"Yeah, but politicians on both sides lie."**
I thought that Holan's methods could help me argue that not every politician lies to the same degree.

To measure how much a given politician lies, Holan tallied the results of PolitiFact’s fact checks for that person between 2007 and 2015. The obvious weakness of this approach is that the samples for each politician might not be equally representative. For example, perhaps Ben Carson has a higher rate of lying than Marco Rubio because PolitiFact simply scrutinized him more closely. If Politifact kept searching, isn’t it possible that they might find more Rubio lies? Holan addresses this directly:

> We don’t check absolutely everything a candidate says, but focus on what catches our eye as significant, newsworthy or potentially influential. Our ratings are also not intended to be statistically representative but to show trends over time.

This is not a criticsm of PolitiFact's methods: they choose to invest their time checking politicians' most important and noteworthy claims.
But to compare two politicians' lying, I need a different strategy.

## Brandolini's Law

I want to know: How often does each politician lie? 
But how can I possibly answer that question?
PolitiFact's haphazard sampling won't work for me.
But short of mic’ing every politician and hiring a small army of fact-checkers to verify every word, what else could I do?

What we're fighting is [Brandolini's Law](https://en.wikipedia.org/wiki/Brandolini%27s_law):

> The amount of energy needed to refute bullshit is an order of magnitude bigger than that needed to produce it.

Every week there's a new press conference, a new podcast appearance, a hundred new tweets.
It would be impossible to fact-check everything.

So let's revist sampling but take a different approach.

## Sampling

We've established that it would be impossible to continually check every claim that a politician makes.
However, if we properly evaluate a sample, maybe we don't need to.

**Let's use *an entire speech* as a sample and fact-check *every declarative sentence***.

Investing the time to exhaustively fact-check a lengthy sample of text allows us to establish a rate of lying.
Once we have this, we can allow ourselves to detach from the firehose of new content.

The goal is that my next conversation on this topic goes something like this:
> Q: "Did you listen to so-and-so's new podcast episode?"
> A: "No, but his last one was 60% lies, so I don't feel the need to."

## RFK Jr. and Pete Buttigieg

To demonstrate this, I fact-checked two speeches: [one from RFK Jr. about autism rates](https://www.youtube.com/watch?v=ZUq0GLvgqRs) and [one from Pete Buttigieg about railway safety](https://youtu.be/tCvozJkvU0k?t=164). They are both official press conferences from cabinet secretaries.

I went through the transcripts of both speeches sentence by sentence.
I marked each factual claim, evaluated it, and labeled it as true, false, or misleading:

{{< figure src="/media/fact-checking/sample.png" alt="Example fact check document" caption="" class="big" >}}

You can read my annotated transcripts of [RFK Jr.'s](https://fact-check.brady.fyi/documents/3f744445-0703-4baf-8925-8fe8f5937462) and [Buttigieg's](https://fact-check.brady.fyi/documents/daceccbe-2c3d-4519-8c79-dce01f173536) speeches.

The graphics below show the results.
The graphic shows the duration of the speech from left to right.
Red and yellow bars indicate false claims; blue bars indicate true claims.

This graphic represents RFK Jr.'s speech on autism rates on April 16, 2025.

{{< figure src="/media/fact-checking/rfkjr.png" alt="Results of the fact check on RFK Jr's speech" caption="" class="big" >}}

This graphic represents Pete Buttigieg’s speech on railway safety on April 2, 2024.

{{< figure src="/media/fact-checking/buttigieg.png" alt="Results of the fact check on RFK Jr's speech" caption="" class="big" >}}

## Conclusion

On average, when RFK Jr. speaks, he tells more than eight lies every five minutes.
On average, almost 60% of his claims are false.
I cannot continually fact-check every new thing he says, but I can reference these rates when considering new claims he makes.

And is this the same for every other politician?
No.
You can see in this example that RFK Jr's rate of lying is meaningfully different than Pete Buttigieg's.

## FAQ

#### Don’t you still have a sampling problem? Couldn’t you have just picked a speech where RFK Jr. lied a lot?

Both of these speeches were given behind the seal of the White House.
There's no reason to think they do not represent the best these politicians have to offer.

#### What sort of lies were these?
[RFK Jr.'s falsehoods](https://fact-check.brady.fyi/documents/3f744445-0703-4baf-8925-8fe8f5937462) were:
* Referencing tables in scientific papers that were irrelevant to his claim
* Citing the wrong numbers from scientific papers
* Misrepresenting the conclusions of the papers he referenced
* Citing retracted papers

[Buttigieg's falsehoods](https://fact-check.brady.fyi/documents/daceccbe-2c3d-4519-8c79-dce01f173536) were:
* Exaggerating (saying "tens of thousands" when the number was 13,000)
* Making a broad, unverifiable claim about historic trends
* Using the term "99%" too casually

#### Did AI do the fact checking?

No. I did it myself, and it took a long time. However, by doing this properly once, I don't need to do it continually.

I did occasionally use ChatGPT as a search engine while fact-checking.

#### Aren't you just nitpicking?  Even if there are falsehoods in individual sentences, couldn’t the overall argument still be true?

That’s up to you to decide, and it’s easier to decide when you know whether the individual sentences are true.

If you're looking for a rebuttal to RFK Jr.'s argument, [PBS did a great job](https://www.pbs.org/newshour/politics/fact-checking-robert-f-kennedy-jr-s-statements-on-autism).

#### Where can I learn more about this?

Check out [this paper](https://journals.sagepub.com/doi/10.1177/2053168019870351) on the effects of summary of fact-checks.
