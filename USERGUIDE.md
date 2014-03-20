# Cypherfunk Tip Bot

This guide is based on the excellent [Reddcoin tipbot documentation](http://www.reddit.com/r/reddCoin/wiki/tipbot). All credit for the  software goes to the creators of [Reddit ALTcointip](http://www.reddit.com/r/ALTcointip/), currently released under GPL v2.

### Warning

This service is in early BETA. This service is provided "as is" without warranty of any kind, either express or implied, including, without limitation, the implied warranties of merchantability, fitness for a particular purpose, non-infringement, error-free or uninterrupted service. You are using this service at your own risk; in addition, the coins in your account are only as secure as your Reddit account is. Do not hold large sums of coins here; simply withdraw or tip others.

## Introduction

The Cypherfunk Tip Bot ([FUNKTipbot](http://www.reddit.com/user/FUNKTipbot)) is a service provided for free by the Cypherfunk community that allows you to easily give (tip) another Reddit user some Cypherfunk (FUNK).

The Cypherfunk cryptocurrency was created to allow listeners tip their favourite independent musical artists online, so that they may continue to create and release music without having to go through the trouble of being signed by a label.

The bot allows you to store Cypherfunk coins in a wallet dedicated to Reddit tipping, and hand out tips to any other Reddit user with a single command, whether they have previously registered with the service or not.

For more information about The Cypherfunks, both the decentralised band and the cryptocurrency, check out [the official site](http://thecypherfunks.com/). The Cypherfunk philosophy is outlined [on the blog](http://blog.thecypherfunks.com/philosophy).

## Usage instructions

### Tipping
To send a tip, you need to first register with the tip bot, then deposit some Cypherfunk, and finally leave your tip by simply leaving a properly formatted comment for the person to whom you want to gift some FUNK.

### Registering
Go to the bot's user page by clicking "FUNKTipbot" just above, and send it a message with subject "register" and body "+register". [Here's a pre-filled out form](http://www.reddit.com/message/compose/?to=FUNKTipbot&subject=register&message=%2Bregister) for your convenience. Up to a couple of minutes after you send the message, you will receive one back to confirm that you're now registered with the bot.

### Depositing
In order to use the tip bot, you first need to deposit some Cypherfunk. If you don't know how to get FUNK, your easiest bet is to trade Bitcoins for them on an exchange. The first cryptocurrency exchange to support Cypherfunk is [Crypto Rush](http://cryptorush.in/).  Other than purchasing, you can mine Cypherfunk using GPUs or scrypt ASICs. See [the announcement thread on Bitcoin Talk](https://bitcointalk.org/index.php?topic=469407.0) for links to mining pools and more.

To deposit, find your deposit address by sending the bot a message with [subject "info" and body "+info"](http://www.reddit.com/message/compose/?to=FUNKTipbot&subject=info&message=%2Binfo). You will receive back a message that contains your current balance and deposit address. Simply send coins to the address you see, and the bot will make them available for you to spend on the site!

### Sending a tip
Simply leave a comment in reply to the user you'd like to tip, with something along the lines of the following:

    +/u/FUNKTipbot {number} funk

Replace `{number}` with the quantity of Cypherfunk you'd like to give the recipient. Within a couple of minutes, the tip bot should leave a comment in reply verifying that the tip has been sent correctly. Don't worry that the user may not be registered with the tip bot, they can register after they have been tipped and still access what you gave.

## Commands

[+register](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=register&message=%2Bregister): create an account. The bot will generate a unique cryptocoin address for each supported coin, and send you that info.

[+info](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=info&message=%2Binfo): get information about the account: unique coin addresses, balances.

[+redeem](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=redeem&message=%2Bredeem): redeem your karma! reddtipbot bot will deposit some coins to your account based on formula below. You can only do this once!

    amount = $0.03 + (link_karma × $0.00002) + (comment_karma × $0.000002)

[+withdraw](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=redeem&message=%2Bwithdraw ADDRESS [AMOUNT|KEYWORD]): tell the bot to send Reddcoins to a given address. Its syntax is:

    +withdraw ADDRESS [AMOUNT|KEYWORD] COIN

>     Note: Network transaction fee is automatically added to when sending to an address. For example, if you ask to withdraw 1 Reddcoin, your total withdraw amount will be 1.001 Reddcoin, out of which 0.001 Reddcoin will go towards transaction fee. Reddtipbot bot does not keep transaction fees - they go to the network as a payment for processing the transaction.

[+accept](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=accept&message=%2Baccept): accept all pending tips. If you've received a tip before you've registered with the bot, it's marked as pending until you +accept or +decline it. Pending tips expire in 48 hours.[

[+decline](http://www.reddit.com/message/compose?to=FUNKTipbot&subject=decline&message=%2Bdecline): decline all pending tips. If you've received a tip before you've registered with the bot, it's marked as pending until you +accept or +decline it. Pending tips expire in 48 hours.

### Tipping

[+/u/FUNKTipbot]: The main command, used to tip other users or send tips directly to a given address. The basic syntax is:

    +/u/FUNKTipbot [@user|ADDRESS] [AMOUNT|KEYWORD] funk

The second parameter is only needed if you are sending the tip using a PM directly to the tip bot, rather than commenting on a post by another Reddit user.

### Error conditions
If the bot is unable to either understand the message, or process it due to an internal error, it will send a message confirming the failure to the originating user. 

If the bot does not reply to a comment, check your inbox. If nothing has arrived within 10 minutes of you sending a message to it or leaving a tip, please contact the Cypherfunk Developers on [the Cypherfunk subreddit](http://www.reddit.com/r/thecypherfunks).

### Further information
Check out the [ALTcointip wiki](http://www.reddit.com/r/ALTcointip/wiki/index) for detailed information on usage.