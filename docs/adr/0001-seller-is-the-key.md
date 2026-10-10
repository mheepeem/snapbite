Title - ADR 1: seller is the key, not location

Status - Accepted

Context - Seller set the price for food and location can only identify food and price effectively in case of dine in, so how can we handle the case of delivery? and how about dine in case but that location is food court? this mean more than one seller can sell the same thing.

Decision - we will focus on getting information from seller instead of location, this solve problem that location can't. for dine in we will get seller information by using GPS and in case of location have a lot of seller, we will use other variable such as nearby seller and settle for the price and if there are still other seller that sell the same thing we will create a choice that add one extra step or none at all if suggestion correct for user to choose. for delivery we will get information from seller name and other information via screenshot because we can't get the location directly from delivery app.

Consequences - We have 2 routes to handle, dine-in and delivery. if we can't determine the seller we may need to fallback to manual input step and introduce the same problem that make me don't want to record. In case of food court if suggestion give me the wrong one , this mean an extra step do to. and how we store data will got effect because in case of delivery, it may miss detail of food in some case, like I don't get the picture or need to decide later to take a picture after got one or not. Price need to be handle in both lookup and record way because price got effected all the time depends on other factor, lookup and make suggestion first if it's not true,  I make extra step to corrected it.
