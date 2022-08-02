# Design-and-Development-of-Smart-Contract-in-Auction-for-Fundraising-for-a-Social-Cause

PROBLEM STATEMENT :

Consider the problem of Chinese auction or penny social. We will refer to it as a simple “Auction.” It is a conventional approach used for fundraising for a cause. The organizers collect items to be auctioned off for raising funds. Before the auction, the items for auctions are received and arranged each with a bowl to place the bid. A chairperson is a special person among the organizers. She/he heads the effort and is the only person who can determine the winner by random drawing at the end of the auction. A set of bidders buy sheets of tickets with their money. The bidder’s sheet has a stub that identifies the bidder’snumber, and tokens bought. The bidders examine the items to bid, place the one or more tickets in the bowl in front of the items they desire to bid for until all the tickets are used. After the auction period ends the chairperson, collects the bowls, randomly selects a ticket from each item’s bowl to determine the winning bidder for that item. The item is transferred to the winning bidder. Total money collected is the fund raised by the penny social auction.

ASSUMPTIONS :

Fixed number of bidders, initialized to 4. All 4 need to self-register. Funds transfer from bidder is automatically done and is not in the scope of this application.
Fixed number of items to be auctioned off, initialized to 3.
Items auctioned are indexed from 0..N-1 where N is the number of items for auction. N is 2.
Each bidder buys just 1 sheet of tickets or tokens; each sheet has only 5 tokens.
Assume simple number for the serial numbers for the sheet of tickets: 0,1,2,3. Here we show the tokens of bidder 0 and 1.

The Design:

Let’s design the smart contract for this. Visualize the situation using the screen shot given below.

These are the pictures of items, we need to define “Items” in the smart contract. We will also need to
define Persons or bidders who will bidding on the Items. We will also need some supporting data
variables.
The functions are similar to the Ballot of our lessons. Constructor that initializes the owner, register that
allows (decentralized person) to register online to get the tokens and start bidding, bid function that lets
a person bid, and finally revealWinner, to randomly choose the winner for the item auctioned. Here is
our design. Always remember to design first. The Auction smart contract has Item and Person structs
and other data items such as array of Items, array of Persons, array of winners, mappings, and
beneficiary address.
<img width="189" alt="image" src="https://user-images.githubusercontent.com/77969439/182459018-7dba283e-b6ec-4cba-ae24-59874d43dd8a.png">
<img width="314" alt="image" src="https://user-images.githubusercontent.com/77969439/182459138-03342770-c148-4e04-aba1-9e4e812992b3.png">


