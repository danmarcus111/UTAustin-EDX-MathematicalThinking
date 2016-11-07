# A shakey story

Sam and Stacey are a couple at a party, where 4 other couples were present.  At the party anyone can shake anyone's hand, but no-one will:

a. shake their own partner's hand; or

b. shake their own hand.

At the end of the night, Sam talks to the people outside his couple and found that each person had shaken a different number of hands.  One person had shaken 0, one had shaken 1, one had shaken 2 all the way up to 8.

Can Sam work out how many hands his partner Stacey had shook?

## Attempt a simpler problem

What if we say there is only one couple?  It is a ludicrously simple example, but maybe it could provide an insight.

We know in this case that Stacey must have shaken zero hands.

What if there were two couples, Sam asks the other 3 people (including Stacey) and finds that the answers are 0, 1, 2.  

What if Stacey shook 2 hands?  We know that one of the people in the other couple shook zero hands and Stacey can't shake Sam's hand, so we can rule this out.

What if she shook zero hands?  No-one from the other couple could shake two hands, because they can only shake Sam's hands.  This is therefore impossible.

So we know she must have shaken one hand.  We can test this makes sense.  She shakes one of the other couple's hand who also shakes Sam's hand (that 2).  The other person in the other couple shakes 0 hands.  This therefore works.

What insights do we have?  Well we know that the couple's hand shaking looks like this (0,2), (1,1).  Is it a coincidence that the lowest hand shaker is a couple with the highest hand shaker?  It's not - because if one person in a couple has shaken everyone's hand and there is someone who has shaken 0 - that must be the other person in that couple.

## Iteration

Let's increase the number of couples and apply this knowledge.

We now have 3 couples, and we know that each of the 5 people asked answer 0, 1, 2, 3 and 4 respectively.

We know that (4,0) must be a pair.  And that means everyone else (including Stacey) has shaken at least one hand.

We are now left with the original problem again.  We are left with 3 people, one of which shakes 0 more hands, another shakes 1 more hands and another shakes 2 more hands.  So we pair up the (2,0) (who are really (3,1)) and we know Stacey must have shook one more person's hand.  Stacey shook 2 hands.

Can we apply this to the original question?

Yes - we know that we get the answers 0,1,2,3,4,5,6,7,8 .  The other couple's must shake (0,8), (1,7), (2,6), (3,5).  This means Stacey must have shaken 4 hands.







