# Ravenhyde-RavensTinyShopAdds

**Welcome to Ravenhyde's Tiny Shop Additions!**

The premise of this mod is that six of the shops carry an extra item or two related to their main inventory. This item is random - you might see something relatively worthless one day and an expensive item the next. The shopkeepers know you can pay, so they're happy to carry extra stuff for you. Sometimes their prices even fluctuate, so you might find an item cheaper or more expensive the next time it shows up.

The shops affected and their items are as follows:

* Clint's: Clint now carries a random gem or mineral.
* Pierre's: Pierre now carries an extra fruit, vegetable, or flower. If you get lucky, he might even carry a better quality item!
* Willie's: Willie now carries a random fish.
* Marnie's: Marnie now sells a random standard animal product.
* Robin's: Robin now carries a random machine, sprinkler, or chest.
* Adventurer's Guild: Marlon's shop now sells a random weapon.


**Installation:**
This mod requires Content Patcher and Stardew Valley 1.6 to work. It will not work in prior versions of the game. If you are running 1.5, I have a similar mod (Hat Mouse Extra) that uses Shop Tile Framework and Content Patcher.

If you want all six shops, install the folder "[CP]RavensTinyShopAdds" to your mods folder.

If you want just one or some of them, the folder "Individual Shops" has a mod for each shop, labeled by the owner's name (or Marlon, for the Adventurer's Guild). So if you wanted to install just the ones for Marnie's and Clint's shops, you'd copy "[CP]RavensTinyShopAddsMarnie" and "[CP]RavensTinyShopAddsClint" to your mods folder.

Installing both the full mod and the individual shops shouldn't cause any conflicts, but they're not intended to be installed together.

**FAQs:**

**How cheaty is this mod?**

It's not really something I'd consider "Fair and Balanced" but it shouldn't be overly unbalancing either. The default setup allows one item per player per day. That being said, here's why each of the shops could be unbalanced:

-Clint's shop allows a player to buy a missing mineral for the museum (or if you get very very very lucky, carries the prismatic shard). 

-Pierre's shop carries some items for the Community Center, including a chance of carrying a gold-star fruit/vegetable.

-Willy's has a small chance of carrying the legendary fish, including some of the late game quest ones. 

-Marnie's carries animal products. Of all the shops, hers is the most balanced and the most aimed at Community Center completion, though you can likely get chicken/duck eggs cheaper than buying chickens or ducks.

-Robin's shop carries a lot of the craftable machines (including those learned by leveling up in skills) though not anything requiring Mastery. She also carries sprinklers and chests.

-The Adventurer's Guild has a chance of carrying the Galaxy weapon series, though not anything more powerful.

In addition, by default these are set to allow one per player (allowing multiple people to buy potentially powerful items) rather than one per farm.

(You still have to catch any fish/make any craftables for Perfection; these items won't help with that.)

**Does it work in multiplayer?**

I can't see why not! It's a Content Patcher mod, which means that if you don't have the mod you won't be able to use it where another person could. I haven't been able to test as I don't use multiplayer.

**Does it work with expansion mods?**

I've only tried it with Stardew Valley Expanded, but had no issues so far. The three shops that carry categories of items (Pierre, Willie, and Clint) will carry the new items in their defined categories. There is a remote possiblity that if one of the items in an expansion mod does not have a sell price for some reason (this only applies to items one of those three shops would sell) as this would cause the item to be free.

**I want the shops to sell two items per day/I only want one purchase per farm:**

I'm currently not set up for Generic Mod Config Menu (it's on my list of things to do but not high-priority), but some things can manually be changed.

-The line "MaxItems" sets the number of additional items each shop sells; the default is 1. 
-The line "AvailableStock" sets how many of each item you can buy per person; the default is 1.
-The line "AvailableStockLimit" can be changed from "Player" to "Global" if you want to limit to a farm-wide basis. 

Note that these lines apply on a per-shop basis; setting things so Clint sells 2 items a day will not have an effect on Marnie's shop.

If you are confused as to the difference between MaxItems and AvailableStock, here's an example:
- You set MaxItems to 2 and AvailableStock to 1. When you open the shop menu, you can buy one each of a ruby an a pyrite.
- You set MaxItems to 1 and AvailableStock to 2. When you open the menu, you can buy up to 2 pyrite but Clint isn't stocking rubies today.
- You set MaxItems to 2 and AvailableStock to 2. When you open the menu, you can buy 2 rubies and 2 pyrites.

As for how AvailableStockLimit would work:
Clint's item of the day is a diamond. There are four players on the multiplayer farm.
- with the setting "Player", all four players could buy a diamond.
- with the setting "Global", once player A had bought the diamond, it wouldn't be available to purchase for players B, C, and D.d

**I think that the shops are selling items too cheaply.**

This is a legitimate concern! For the most part, the mod is using the game's price data and multiplying it by one of several amounts. If you want to make things more expensive, look for "RandomAmount" under "PriceModifiers", remove one or more of the lower numbers, and add higher numbers. (So if a shop lists [5, 10, 15, 20] you could change that to be [10, 15, 20, 25] instead.)

If you want a seller to sell at a consistent markup (for example, you wanted Robin's shop to sell items at 20x the price given in the game), you would substitute "Amount": 20.0 (or whatever multiplier) for the "RandomAmount" section.

**Anything else of note? Any trivia?**

- Pierre is the only one who can sell more than one item under the default settings due to the way that gold-quality crops had to be set up in the code. By default, he has a 10% chance of selling a gold-quality crop.
- Robin's inventory includes a small glow ring because I hate navigating levels 31-39 so much.
- There are a surprising amount of items that don't have a sale price in the game. I was a little surprised when I was testing and Robin sold me a Worm Bin for 0. This is why the main mod and the mod set up for Robin's shop has a separate section so I could add base prices for a couple of items.
- Willy and Clint sell everything under a certain category; Pierre mostly does the same, except he has a chance of randomly selling a gold-quality item as well. Robin, Marnie, and the Adventurer's Guild have defined lists because otherwise they were selling items that didn't fit in with my idea of what they would sell, especially in early game.
