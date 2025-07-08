---
title: "Battling Brandolini's Law with Sampling"
date: "2025-07-08"
---

*[Brady Hurlburt](/) - July 8, 2025*

## "All Politicians Lie"

In 2015, Angi Drobnic Holan published [a wonderful article titled "All Politicians Lie. Some Lie More Than Others."](https://www.nytimes.com/2015/12/13/opinion/campaign-stops/all-politicians-lie-some-lie-more-than-others.html)
In it, she makes that case that while all politician's lie, there are meaningful differences in the amounts that they do so.

{{< figure src="/media/fact-checking/nyt.png" alt="Holan's analysis of PolitiFact lyting rates from her NYT article" caption="" class="big" >}}

Her article resonated with me.
In conversations with my friends, when I've called out a policician's lie, I'm sometimes met with **"Yeah, but politicians on both sides lie."**
I thought maybe Holan's methods could help me argue that not every politician's lying is the same.

As a metric for amount of lying, Holan uses the counts of Politifact checks by result.
The obvious weakness of this approach is this: **couldn't Politifact simply have checked more of Ben Carson's lies than Mitt Romney's?**
If they wanted to, couldn't they find more Romney lies?
Holan addresses this directly:

> We don’t check absolutely everything a candidate says, but focus on what catches our eye as significant, newsworthy or potentially influential. Our ratings are also not intended to be statistically representative but to show trends over time.

This is not an criticsm of Politifact's mission: they choose to invest their time checking the most important claims they can find.
But it's not going to work for me.

## Sampling

I want to answer questions like "Is this public figure a liar?" and "Should I listen when they talk?"
What can I do?
Hook a microphone to every politician and assign a team of 100 to fact check every word?

Let's do what we do when we have too many things to count or classify: let's sample.
Let's consider an entire speech from a politician and fact-check ***every declarative sentence***.

## How this helps us fight Brandolini's Law

> The amount of energy needed to refute bullshit is an order of magnitude bigger than that needed to produce it. - Brandolini's Law

As Brandolini's Law points out, it would be impossible continually to check every claim that a politician makes.
But, once we've evaluated a sample, maybe we don't need to.

Investing the time to completely and exhaustively fact check a lengthy sample of text allows us to establish a rate of lying.
Once we have this, we can allow ourselves to detach from the firehose of new content.

The goal is this:
> Q: "Did you listen to so-and-so's new podcast episode?"
> A: "No, but his last one was 60% lies, so I don't feel the need to."

## RFK Jr. and Pete Buttigieg

To demonstrate this, I fact-checked two speeches: one from RFK Jr. and one from Pete Buttigieg.

I fact-checked like a newsroom fact-checker would. This means:
* This is not strictly an analysis of the overall arguments ([PBS and many others already did a great job at that](https://www.pbs.org/newshour/politics/fact-checking-robert-f-kennedy-jr-s-statements-on-autism)). This is a count of how many individual sentences were lies.
* I did not evaluate whether a false claim worked for or against the overall argument. I only considered whether it was true or not.

In the graphics below, the width of the rectangle is the duration of the speech.
Red and yellow sections mark false claims; blue sections mark true claims.

Here is the result of fact-checking **RFK Jr's** Health and Human Services press conference on autism rates on April 16, 2025.
[You can read my full fact-check here](https://fact-check.brady.fyi/documents/3f744445-0703-4baf-8925-8fe8f5937462).

{{< figure src="/media/fact-checking/rfkjr.png" alt="Results of the fact check on RFK Jr's speech" caption="" class="big" >}}

Here is the result of fact-checking **Pete Buttigieg's** press conference on railway safety on April 4, 2022.
[You can read my full fact-check here](https://fact-check.brady.fyi/documents/daceccbe-2c3d-4519-8c79-dce01f173536).

{{< figure src="/media/fact-checking/buttigieg.png" alt="Results of the fact check on RFK Jr's speech" caption="" class="big" >}}

## Conclusion

On average, when RFK Jr. speaks, he tells more than eight lies every five minutes.
On average, almost 60% of his claims are false.
I cannot continually fact check every new thing he says, but I can reference these rates when dismissing new claims he makes.

And is this the same for every other politician?
No.
You can see in this example that RFK Jr's rate of lying is meaningfully different than Pete Buttigieg's.

## FAQ

#### Don’t you still have a sampling bias problem? Couldn’t you have just picked a speech where he lied a lot?

Both of these speeches were given behind the seal of the White House.
There's no reason to think they do not represent the best these politicians have to offer.

#### What sort of lies were these?
[RFK Jr.'s falsehoods](https://fact-check.brady.fyi/documents/3f744445-0703-4baf-8925-8fe8f5937462) were:
* Referencing tables in scientific papers that had nothing to do with the claim he was making
* Citing the wrong numbers from scientific papers
* Mis-representing the conclusions of the authors of the papers he referenced
* Citing retracted papers

[Buttigieg's falsehoods](https://fact-check.brady.fyi/documents/daceccbe-2c3d-4519-8c79-dce01f173536) were:
* Exaggeration (saying "tens of thousands" when the number was 13,000)
* A broad, unverifiable claim about historic trends
* Claiming "99% of comments were positive", when it wasn't quite that high

#### Did you use AI to do the fact-checking?

No. I did it myself, and it took a long time. But, my point is that by doing this properly once, I don't need to do it continually.

I did occasionally use ChatGPT as a search engine while fact checking.

#### Aren't you just nitpicking? You’re just looking at problems with individual sentences. Couldn’t his whole argument still be true?

That’s up to you to decide, and it’s easier to decide when you know whether the individual sentences are true.

#### Where can I learn more about this?

Check out [this paper](https://journals.sagepub.com/doi/10.1177/2053168019870351) on the effects of summaries of fact-checks.
