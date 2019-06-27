# Chapter One: The Power of Randomness

#### _Why we do what we do_

**_Version: 2019-06-26 Release 1.0.0_**

## Introduction to Randomness

Cryptographers love randomness.

They love numbers that are entirely unpredictable, where there’s an equal probability that any number will be selected, and where that selection occurs independently of anything else.

Here’s why.

### The Power of Large Numbers

Imagine your Bitcoin (or other digital assets) as being held in a near-infinite set of lockers. Anyone can see what’s in a locker, and anyone can put money in a locker, but each locker is secured with a combination lock, and only the person with the combination can retrieve the money.

One standard type of combination lock has four digits that each run from 0 to 9. That creates 10^4 combinations or 10,000. Here’s where the randomness comes in: if the combination is actually unpredictable, then it can only be broken by someone running through all the possible combinations: 0000, 0001, 0002, etc. If they could test a number a second, they’d break the combination in at most three hours (and on average, in an hour and a half).

Clearly, that’s not sufficient to protect actual money (like cryptocurrencies), especially when attackers can test numbers secretly (over the internet). For that, you need a much larger secret number.

### The Weakness of Passwords

“So,” you might say. “Does that mean that I can use a password to protect my digital assets? Then I can keep it in my head.” Unfortunately, there are multiple problems with this methodology. First, a “brain wallet” is innately prone to failure; worse, there won’t be any way for your heirs or descendants to reclaim your digital assets. However, one more sobering fact makes this methodology even more problematic: traditional passwords are no longer secure.

Theoretically an eight-character password contains 64 bits of randomness, but that turns out not to be the case in reality. That’s because any character in a password is likely to be drawn from the 100 or so characters available on a standard keyboard: that immediately drops the 8 bits of randomness for each character down to 6 or 7, which would be 48 to 56 bits total for an eight-character password. But, passwords are worse than that. They tend to be arranged into words, and they tend to use standard substitutions, which makes them even less secure; like that four-digit locker combination, any short-to-medium-length password can be broken today in a fairly short amount of time!

The [*zxcvbn*](https://github.com/dropbox/zxcvbn/blob/master/README.md) [*interactive password demo*](https://lowe.github.io/tryzxcvbn/) allows the testing of passwords, with results shown for computers of various powers. Obviously *real* passwords should not be tested on any internet service, but the following benchmarks for entirely random passwords of different lengths are instructive. Each entry shows how long the password would take to crack given a machine that could make 10B (billion) guesses a second, which turns out to be a [*realistic goal*](https://arstechnica.com/information-technology/2012/12/25-gpu-cluster-cracks-every-standard-windows-password-in-6-hours/):

* 5 characters (58T%n): less than a second 
* 8 characters (lVA\#6jx6): less than a second 
* 12 characters (G%6L3Y!5cvjC): 2 minutes 
* 16 characters (g0oY!yXZg2Emn\#3z): 12 days 
* 18 characters (K1cAhiQ00I@Ol!vvvK): 1 year 
* 20 characters (EoQ7\^\#y1xR\^WeQeqdst\$): centuries

And that’s why you’re not going to be brain-walleting a password for your digital assets: there’s not enough randomness in a password for it to be well-protected unless it’s very long and fundamentally impossible to memorize. Oh, you could use an alternative like the [*EFF’s randomphrase list*](https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases), which allows you to get the equivalent of 77 bits of protection with six seven-character words. But even in these situations, you’re unlikely to manage more than 80 bits of entropy, which is the absolute minimum you’d want in the current day and age.

At the moment, 80 bits of protection are theoretically safe under any likely cracking scenario … but the Bitcoin mining network as a group actually passed the ability to make 2^80 guesses in a year at the end of 2013 and has [*peaked at closer to 2^92*](https://crypto.stackexchange.com/questions/13299/is-80-bits-of-key-size-considered-safe-against-brute-force-attacks/13305#13305). Though it’s unlikely that someone could put together that much computing power to break a single key, that amount of computer power does already exist on Earth, and we wouldn’t want our assets’ safety lying so near the ever-advancing line of what can be broken.

Which is why it’s fortunate that Bitcoin’s virtual combination lock isn’t 80 bits long, but rather 256.

### The Power of 2^256

A 256-bit private key is a string of 256 ones or zeros, which, requiring 2^256 guesses to step through all of the possibilities, but that doesn’t illustrate the whole scope of the number. We can bring it down to Earth by breaking it down as:

> 2\^32 \* 2\^32 \* 2\^32 \* 2\^32 \* 2\^32 \* 2\^32 \* 2\^32 \* 2\^32

And since 2^32 is a bit more than four billion, this is about the same as:

> 4B \* 4B \* 4B \* 4B \* 4B \* 4B \* 4B \* 4B

So, how hard is that to crack?

#### The Amazon Example

Amazon’s exciting new 3.16xlarge cloud computer, which costs \$25/hour to operate, can compute about 6 billion hashes a second. That only resolves one of those 2^32 multipliers, leaving seven to deal with:

> (4B \* 1.5 = 3.16xlarge computing power) \*

> ⅔ \* 4B \* 4B \* 4B \* 4B \* 4B \* 4B \* 4B

Perhaps we can do better by spending more money: with 21 trillion hashes in an hour costing \$25, the overall cost of using the 3.16xlarge is about \$1 for each thousand billion hashes. Multiply that by the eighty thousand billion dollars circulating in fiat currency, and you can run eighty million billion billion hashes before you bankrupt the whole world.

At this point, you’ve come up with a way to crack an 80-bit secret without using the entire Bitcoin mining network for a year. But, it’s still nowhere near what you need to figure out that 256-bit Bitcoin secret, where you’re still working on that third 2^32 multiplier, with five more to go!

Clearly we have to look beyond the global money supply out into the whole universe to do better.

#### The Universal Example

Let’s take an alternate route and instead consider the entire mining power of the Bitcoin network. That’s been running about 40E in 2019, which is 40 billion billion hashes per second, or 6 billion times as much power as that single 3.16xlarge computer. This deals with two of the 2^32s required to crack a Bitcoin private key, but only by using up what may be the most powerful computer network on modern-day Earth.

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> ⅓ \* 4B \* 4B \* 4B \* 4B \* 4B \* 4B

There are 7.7 billion people on Earth, so let’s give every one of them a magic computer that has the entire power of the current Bitcoin mining network:

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> ⅓ \* ½ \* 4B \* 4B \* 4B \* 4B \* 4B

There are 250 billion stars in the Milky Way (plus or minus 150 billion), so let’s give every star an Earth-like planet where everyone is running magic computers:

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> (4B \* 62 = stars in the Milky Way) \*

> 1/3 \* 1/2 \* 1/62 \* 4B \* 4B \* 4B \* 4B

There are at least 200 billion galaxies in the universe:

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> (4B \* 62 = stars in the Milky Way) \*

> (4B \* 50 = galaxies in the universe) \*

> 1/3 \* 1/2 \* 1/62 \* 1/50 \* 4B \* 4B \* 4B

And finally, it’s been 13.7 billion years since the Big Bang, which is 432 million billion seconds.

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> (4B \* 62 = stars in the Milky Way) \*

> (4B \* 50 = galaxies in the universe) \*

> (4B \* 108M = lifetime of the universe) \*

> 1/3 \* 1/2 \* 1/62 \* 1/50 \* 1/108M \* 4B \* 4B

If you rearrange the fractions, what’s left is:

> 1/500 \* 1/4B \* 4B \* 4B

Or:

> 1/500 \* 4B

Or:

> 8M

In other words, in order to guess all of the possible combinations in a Bitcoin private key, you’d have to have every star in the whole universe have an Earth-like planet where every person had their own complete Bitcoin mining network, and they’d all have to calculate for the entire lifetime of the universe, and then they’d have to do that 8 million more times!

Lucky you, on average you’ll find the key in half of that, or 4 million times!

Which is why cryptographers like randomness.

(And why the 256-bit private key is a lot better than your 12- or 16-character password.)

### The Power of 2^160

Actually, the power of that 256-bit private key is so huge that Bitcoin itself doesn’t use all of it. It instead hashes the public key of its keypair down to a 160-bit Bitcoin address. This *does* decrease the security, because now there are many collisions when converting from that 256-bit keyspace to this smaller 160-bit hashspace. But the number is still so hugely large that it doesn’t matter.

2^160 is only:

> 2\^32 \* 2\^32 \* 2\^32 \* 2\^32 \* 2\^32

But that still means:

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> (4B \* 108M = lifetime of the universe) \*

> 1/3 \* 1/2 \* 1/108M \* 4B

Or:

> (4B \* 4B \* 3 = Bitcoin mining power) \*

> (4B \* 2 = population of Earth) \*

> (4B \* 108M = lifetime of the universe) \*

> 6172

To break a 160-bit hash would require everyone on the Earth to have a computer with the power of the Bitcoin mining network and to run for six thousand times the lifetime of the universe.

Note that the reduction from the 256-bit private key to the 160-bit hash is not a requirement of Bitcoin (or any similar digital-asset system). It’s simply how Bitcoin does things right now, as part of a balance between minimizing storage space while maintaining security that’s at the moment well, well past borderline or reasonable protection

## The Danger of Randomness

However, randomness isn’t easy.

Humans are very bad at picking random numbers. Multiple studies have shown that [*playing rock-scissors-paper is somewhat predictable*](https://www.psychologytoday.com/us/blog/the-blame-game/201504/the-surprising-psychology-rock-paper-scissors), and that’s just humans picking among three numbers. Picking larger random number isn’t any easier (quite the contrary).

And computers aren’t much better at picking random numbers. In fact, they literally can’t. To generate a pseudo-random number, a computer needs to start off with a random number as a seed, which creates a chicken and egg problem. There are certainly ways to resolve this, from the simple idea of seeding a pseudo-random number generator off of the current time to creating true randomness using stochastic natural processes such as thermal noise.

But, it’s tough. And it’s easy to mess up.

Here’s another sobering reality: if a computer process messes up a single bit, then the number of possible guesses is reduced by half. And it doesn’t tend to be just a single bit that’s messed up! When we were doing security reviews of SSL products in the ’90s, we found that about half the products failed the review due to a failure of randomness! Sometimes it’s due to programming errors that entirely eliminate randomness, sometimes it’s due to reuse of randomness (which of course isn’t random), and sometimes it’s due to leaked bits that someone else might know. Every one of these errors *substantially* reduces the randomness: the number of guesses might be reduced by 10x or 100x *or 10 billion times* or zeroed out all together!

So, cryptographers love randomness. But, randomness is hard and needs to be generated carefully.

## The Core of Custody

The \#SmartCustody courses don’t actually talk about *directly* protecting your cryptocurrency: your private key does all that all on its own. In fact, everything that you do with cryptography, from protecting digital assets to signing digital documents, ultimately goes back to that big random number. It doesn’t matter if that number is part of public-key cryptography or a classic symmetric key cryptography system; in either case, the number protects your assets.

What this course instead teaches is how to protect that number: so that you don’t lose it, misuse it, or have it stolen.

That’s all that smart custody is.
