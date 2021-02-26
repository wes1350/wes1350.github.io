---
mathjax: false
tags: Misc
---

# Betting like a Trader: A Superior Betting System

I spent a couple summers in college interning for quantitative trading firms. I no longer work in that industry, but the one thing has stuck with me is the betting system they used. Inspired by the conventions of trading financial instruments, it is simple, flexible, and efficient. If I could, I would *only* use this system when making bets with people.

As an example, here's what a conversation between two people, Alice and Bob, could look like under this betting system. 

> Alice: Hey Bob, at 25 for a hundred that you make that shot.

> Bob: Take 'em!

This translates to a 3:1 bet ($75 vs $25) in Bob's favor (i.e. he would receive the 3x payout), with Bob betting that he makes his next shot.

To explain how this system works, I'll build the concepts from the ground up, with plenty of examples given. Though there's a lot of text, the underlying concepts are simple, and you can skip some examples if you think you've got it down.

## How Does It Work?

You make a bet by *trading* *contracts*. A *contract* is just a base unit for the bet; for now, in order to simplify things, we'll trade one contract at a time. A *trade* means there's a buyer and a seller, i.e. someone who buys the contract and someone else who sells the contract. Don't worry about what exactly all that means yet; we'll get into that soon.


## Contracts

A contract (likely inspired by *futures contracts* in the world of financial instruments) is just (metaphorically) a piece of paper with a certain *value*. The *value* is the quantity we'll be betting on. If what we're originally betting on is non-numeric (e.g. which country wins the next World Cup), we'll give it an appropriate represention to produce an appropriate value.

Here's a (metaphorical) example of a contract:

> This piece of paper is worth $1 for every dollar in my bank account.

As it turns out, I have exactly $800 in my bank account right now. That of course means that this contract is worth exactly $800.

Now remember, we're betting, so you want to make money here. Would you buy this contract for $600, if I offered it to you? You should, considering you'd be buying something worth $800 for only $600 -- a neat $200 profit! 

What about for $900? This time, you should decline -- why pay $900 for something worth only $800? If you're in a negotiating mood, you might counter-offer to buy it for $700 or $750, both of which would net you some profit.

This is of course a bit of a contrived example, so let's look at a slightly more interesting contract, this time in the realm of basketball.

> This contract is worth $10 for every point LeBron James scores in tonight's game.

It's a bit harder to determine the value of this contract, since we don't know exactly how much LeBron will score tonight. Right now, LeBron is averaging about 24 points a game, so the contract is probably worth around $240. If he has an off night, it might end up being worth $150, but if he heats up, it might end up being worth $410. If LeBron twists his ankle at the start of the game, he might score 0 points, making the contract worth $0! With all that in mind, how much are you willing to pay for this contract?

The value of the contract obviously depends on how many points you think LeBron will score tonight. Maybe he's playing against the worst defensive team in the league; in that case, it would probably be worth a bit more than normal, maybe $290 or so, let's say. The better you are at guessing LeBron's point total tonight, the better idea you'll have of what this contract is actually worth.

Let's look at one more example:

> This contract is worth $100,000 if my house (accidentally) burns down this year, and $0 otherwise.

(Hmm... looks an awful lot like insurance, doesn't it?) This is what I call a *binary contract*. Instead of taking on a range of values (like LeBron's point total), it's all-or-nothing: either it's worth $100,000, or it's worthless. How much this is worth is obviously dependent on how likely my house is to burn down this year. If I live in the middle of a very fire-prone forest, this is probably worth a lot, since there's a good chance my house will burn down. On the other hand, if I live in a very rainy area, my house is much less likely to burn down, so it's probably not worth very much.

Let's say my house has a 5% chance of burning down this year. The contract is then worth 5% of $100,000, or $5,000, since on average, the contract pays out $5,000. 


## Trading Contracts

Our betting system is simple: someone draws up a contract and tries to sell it to someone else. They negotiate a price for the contract, and a purchase, or *trade*, happens.

### Trading on Football

Let's see a trade in action, this time about American football:

> Alice: Hey Bob, I have this neat little piece of paper! It says:
> > I, Alice, will give whoever has this piece of paper $100 if the Buccaneers win the Super Bowl this year, and $0 otherwise.

> Alice: Pretty cool, right? Anyways, I'll give it to you for only $40 - a steal!

> Bob: Very interesting, Alice. $40 is a bit steep -- Tom Brady is 43 for God's sake! How about I give you $25 for it?

> Alice: $25? Are you kidding me? I don't care how old he is, it's Tom Brady! $30, take it or leave it.

> Bob: Alright, fine - you've got a deal. $30 it is. 

Let's review what just happened. Alice drew up a contract which pays $100 if the Buccaneers (who have Tom Brady as a player) win the championship this year. In other words, Alice will have to pay $100 to whomever owns that contract if the Buccaneers win. She asks Bob if he wants to buy it, and after some negotiation, they agree on a price of $30 for the contract. Now, Bob pays Alice $30, and in return gets a paper worth $100, but only if the Buccaneers win.

So, now that Bob owns this paper, he's clearly rooting for the Buccaneers to win. If they win, he'll get $100 from Alice, earning him a profit of $70. If they lose, he'll be out $30, since the contract he bought is worthless.

On the flip side, Alice is definitely hoping the Buccaneers lose. If they win, she'll have to pay Bob $100 for a net loss of $70, but if they lose, she gets to keep her $30 without any worries. 

Hopefully that makes sense; they have now wagered, through this contract, on whether the Buccaneers will win. Bob is betting they will win, and Alice is betting they won't. Because of the final price of $30, the payouts are asymmetric: once the outcome is known, Bob will either lose $30, or win $70, and Alice will either win $30, or lose $70.

#### Trade Psychology

Let's take a step back and think about *why* Alice and Bob made this wager, or in other words, traded this contract. If Bob bought it for $30, he must think it's worth *more* than $30, since he's trying to make money through his bet. Maybe he thinks it's worth $31, or maybe he thinks it's worth $81; either way, he definitely doesn't think it's worth less than $30.

Similarly, Alice, having sold the contract for $30, must think it's worth *less* than $30. We don't know whether she thinks it's worth $5 or $25, but she definitely doesn't think it's worth $35. If she did, she wouldn't have sold it to Bob for less than what she thought it was worth.

Note that Bob, having bought the contract, thinks it's worth *more* than $30, while Alice, having sold it, thinks it's worth *less* than $30. Both Alice and Bob think they've made a good deal, but obviously, only one of them is right (unless it's worth *exactly* $30, in which case it's a wash.) Whoever's right will, on average, make a profit.

Let's look at one more example to solidify these concepts.

### Trading on Countries

Alice and Bob meet again. This time, Bob starts it off:

> Bob: Hey, Alice! I heard you just got back from Colombia! How was it?

> Alice: Awesome! I love traveling, some day I'll visit all the countries in the world!

> Bob: Wait, *all* of them? That's gotta be what, 300 countries? There's no way!

> Alice: No dude, it's way less than 300! Can't be more than 250. 

> Bob: Hmm, I'm not so sure about that. How about we bet on it -- If you draw up a contract saying this, I'll buy it from you for $250!

> > This contract entitles whoever holds it to $1 of Alice's money for every country in the world.

> Alice: $250? Well you've got a deal! Let's settle this now; I'll look it up.

> > There are 195 countries in the world today. 

> Alice: That settles it! The contract is only worth $195, but since you bought it for $250, you just owe me $55.

This time, Bob proposed that *Alice* draw up a contract worth $1 for every country in the world, offering to buy it from her for $250. Clearly, if he was willing to buy it for $250, he must have thought there were at least 250 countries in the world; otherwise, he would have been losing money. Alice, since she thought there were fewer than 250 countries, was happy to sell Bob this contract, since she believed she would only pay a smaller amount in exchange.

After looking up the true value of the contract -- $195, or $1 for all 195 countries -- Alice and Bob were able to *settle* the contract, by assigning it a specific value, once they got the necessary information. This time, Alice was the winner: she made money, since her guess for how many countries there were was better than Bob's, as reflected in their agreed upon *trade price*.

## Trading, In Theory and Practice

To make things conceptually simpler, I've used the analogy of buying and selling paper contracts to explain how betting works in this system. The process roughly looks like this:

1. Two people decide on something they want to bet on
2. One person writes up a contract, specifying how much it's worth depending on what they're betting on 
3. Both parties negotiate a price, depending on the to-be-determined value of the contract
4. Once done negotiating, the buyer pays the seller the agreed upon price, receiving the contract in return
5. At some point in time, the contract is settled, giving a final value for the contract
6. The seller pays the buyer the final value of the contract.
7. Depending on the negotiated contract price and the settled contract value, each party will have realized some final profit or loss (potentially $0)

This may seem like a lot of steps, but hopefully it's clear what's going on here. In practice, this process is smooth and quick, and a trade can happen within a couple of seconds. In particular, steps 4, 6 and 7 are rolled up into one: a contract is traded, its value is settled, and whoever loses pays the winner however much they lost. For example, in the second example, Alice and Bob just wait until everything is settled, and then Bob pays Alice $55, his net loss.

Of course, it would be clunky to always have to write up contracts on pieces of paper, so in practice, contracts are exchanged verbally. To further reduce the clunkiness, there are a few terms related to buying and selling:

- *X bid*: an offer to buy a contract for X.
- *at X*: an offer to sell a contract for X.
- *buy/take 'em*: said to a seller to accept their offer to sell (i.e. for you to buy from them)
- *sell/sold*: said to a buyer to accept their offer to buy (i.e. for you to sell to them)

Personally, I prefer saying "take 'em" and "sold" when buying and selling. Also, when saying "X bid" or "at X", the units may be specified later if they aren't clear. To illustrate how these are used, here is what the previous example between Alice and Bob could look like using this terminology.

> (prior conversation)

> Bob: Hmm, I'm not so sure about that. How about we bet on it -- 250 bid on the number of countries, $1 a country.

> Alice: Sold! Let's look this up.

> > There are 195 countries in the world today. 

> Alice: Alright, you owe me $55 then.

Ok, that was much quicker. With a bit of practice, you'll get fast at it very quickly.

Let's highlight one thing in particular: when you're bidding or buying (i.e. saying "X bid" or "take 'em!"), you are hoping the actual value is *higher* than the proposed price: you're "bidding" a lower price for a higher-value item (the contract) in order to make a profit. Similarly, when you're "taking" (i.e. saying "at X" or "sold!"), you're hoping the actual value is *lower* than the price, in order to make a profit.

To drive this concept home, let's look at a few more examples.

### Example: Betting on the World Cup

> Alice: Hey Bob, Brazil's looking pretty strong for this year's World Cup... 20 bid they win the whole thing for $100.

> Bob: Sold! 

In this example, there are a couple of important things to note. First, this is a *binary contract*: either Brazil wins or doesn't. In this case, the contract value is assumed to be 0 (if they lose) or 100 (if they win). Second, since "20" has no units, Alice further specified the size: the contract size is $100, meaning the 20 bid implies a price of $20.

Now let's think about what Alice and Bob are thinking. Alice's 20 bid implies that she thinks that Brazil has at least a 20% chance of winning, and Bob's selling implies that he thinks the chance is less than 20%. The final payouts will be $20 to Bob (if Brazil loses) and $80 to Alice (if Brazil wins). So, by design, there is a 4:1 ratio built-in.

### Example: Betting on Push-ups

> Bob: I've been crushing it in the gym lately. I can definitely do a hundred push-ups now, no breaks.

> Alice: 100? No offense, but there's no way. I'm at 100, $1 a pushup. 

> Bob: Take 'em! Watch this.

> > Bob does 127 push-ups without stopping

> Alice: Wow, I didn't expect that. Here's your $27.

By saying she was "at 100", Alice is betting that Bob can't do more than 100 push-ups. The fewer he does, the more Alice will make.

In a case like this, there's unlimited *downside* for Alice: there's no limit to how much money she could lose, in theory, if Bob never stops doing push-ups. If she wants, she can protect herself by proposing a cap, e.g. a max loss of $50.

### Example: Betting on the Weather

> Alice: Man, it's looking pretty ominous outside. There might be a thunderstorm tonight.

> Bob: Thunderstorm? Here? Tonight? At 40.

> Alice: 40? That's pretty steep. 25 bid.

> Bob: At 30.

> Alice: Take 'em! How much?

> Bob: $20. 

> Alice: Deal.

This time, Alice and Bob negotiate a bit before settling on a price of 30 (out of 100). They end up agreeing on a contract size (i.e. what dollar amount 100 means) of $20, so if it does end up thunderstorming, Alice will win 0.7 * $20 = $14, while if it doesn't, Bob will win 0.3 * $20 = $6. Just to ensure it's clear, the $14 figure if Alice wins is derived from her payment (30% of $20, or $6) subtracted from the value of her winning contract ($20), for a net of $20 - $6 = $14.

## Why This Betting System?

I can't speak for all betting systems, but here are some things I like about this one:

- Flexbility, for binary contracts. You can very easily control the odds (or equivalently, break-even probabilities) by adjusting the price of the contract. A 1 bid gives 99:1 odds, while a 99 bid gives the opposite odds. A 50 bid gives the traditional 1:1 odds.
- Variable profit/loss for continuous (non-binary) contracts. If you buy the number of points (i.e. buy a contract tied to the number of points) LeBron scores tonight, you will earn more money the more he scores. If you prefer a fixed profit or loss, a binary contract does the trick.
- Efficiency, once you have the terminology down. You can quickly say "90 bid" on something, and someone else can take the bet with "Sold!"
- The ability to think directly in terms of probabilities, as opposed to odds. Probabilities are much easier to reason about, when we think about how likely something is to happen.

## Final Thoughts

I love using this betting system, even though it seems only traders and affiliated personnel use it. There's a small learning curve, but I think it's far more elegant than what people generally use. I hope one day that I'll be able to casually make bets with my friends using this system. For now, I'm at 25 that ever happens.
