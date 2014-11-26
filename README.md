# TheftcoinJS

TheftcoinJS is a pre-browserified, pre-minified, and pre-uglified version of [BitcoinJS](https://github.com/bitcoinjs/bitcoinjs-lib) that's ready to get plugged into your client-side Bitcoin app. Just copy one of the two files (your choice) into that wallet app your $700 million valued (privately determined by the investors, of course) Bitcoin startup is building that's totally going to Solve All Security Problems With Using Bitcoin (TM) and Totally Disrupt the Fuck out of Shit (TM), blast some dubstep (or throw an SSD into a blender and set it to liquify), and start raging HARD on [the future of all trade and commerce](https://www.youtube.com/watch?feature=player_detailpage&v=QcUWaVbC8wY#t=227). Watch out Bernanke, $4000 computer chairs in the Mission District soaked in $100 black-truffle burrito grease, your days are numbered bud.

Now when building systems that will be handling potentially millions of dollars worth of Bitcoin (or in Mt. Gox's case, hundreds of millions), you don't even have to conduct the arduous, pain-staking, Andrew Lloyd Webber musical watching, chalk-screeching practice of running three-ish commands (`apt-get install nodejs && npm install && npm run-script compile`) to get a copy of your own derived from auditable, human-readable, version-controlled source code that you can inspect yourself, and that you can run tests on, and add features, and fix bugs, and send those bugfixes back to the project you're basically staking your entire startup's reputation and future on top of.

Oh, and don't worry, it's signed with my PGP key, so you Know It's Secure (trademark filed, still pending, apparently [Zombo.com](http://zombo.com) may have beat me to it).

## What's the catch?

Simple.

One of these files will function as you would expect. Possibly. You probably won't know how to use it, because you refused to `git clone` the [BitcoinJS](https://github.com/bitcoinjs/bitcoinjs-lib) repository to have the source code available for review, because "eww, Node.JS, it has cooties or something, I'm not using that", but that's neither here nor there.

The other file (or both?) will send all money transferred through it to one of my Bitcoin cold storage wallets, where I will proceed to use it to buy tons of PCP, get extremely high on said PCP, take my clothes off and start spraying people driving down the highway with a fire hydrant until the police show up, and use the remaining money to post bail. Or I'll buy some pairs of Alpaca socks for my grandfather on [Bitcoin Black Friday](http://www.bitcoinblackfriday.com), haven't decided which I'm going to do yet. He does like socks. But maybe he would like PCP more...

## Benefits of using this instead of building your own minified version

You don't have to run three or four commands to get the file for your browser-based Bitcoin application, from a local repository that allows you the convenience and accessibility of readable source code, testing, and the ability to fix bugs or add useful features. You can continue to live in your [safe, secure](http://tonyarcieri.com/whats-wrong-with-webcrypto) world of browser-only JavaScript, being content in your ignorance of the science and technology that brought that environment to you, and take solace in the fact that as long as you stay in that world and blissfully ignore the processes that create it, [nothing will ever go wrong](https://bitcointalk.org/index.php?topic=576337).

## Caveats of using one of these pre-built versions

You might lose all your money.

## I picked the wrong one (or both). Can you send me my money back?

No.

## Somebody will figure out a quick way to find it.

Assuredly. [Fedor Indutny](https://twitter.com/indutny) could probably do it in his sleep. I spent exactly one minute making the change(s), and spent zero time obfuscating it, aside from running `npm run-script compile`. In fact, I didn't even test my change(s) to see if it worked.

That's not the point. The point is that the tools we have available to figure out problems with jumbled code are pretty terrible, and the warning signs are not obvious. The point is that Github won't display the source of these files in a nice, cleaned, syntax highlighted way. The point is that you run `diff bitcoinjs-min.1.js bitcoinjs-min.2.js` and you eat more static than Kirk did in Wrath of Khan. With time and patience, someone much smarter than I will ever be could make this much, much harder to figure out. And unlike me, they won't give you a hint there there might be something wrong here.

When you're doing something important like, say, handling other people's money in an incredibly hostile computing environment, don't trust code you can't audit, understand, inspect, write tests against, and fix bugs on.

## But does it have a lock with a checkmark?

Yeah, in the grand tradition of TheftcoinJS, I just stole one from [rbnacl](https://github.com/cryptosphere/rbnacl):

![Checkmarked Lock](http://i.imgur.com/dwA0Ffi.png)

## Parting thoughts

* Please stop asking the BitcoinJS project to bundle a minified, uglified version of BitcoinJS for you. Please, please, *please* build your own from the source code using the `package.json` script that has been provided.

* An indirect attack against NPM or the dependencies is quite possible. And that possibility is amplified by the fact that NPM does not yet support signing modules with PGP keys. This is a fair criticism, perhaps one so damaging that it makes this entire rant irrelevant. But even with `npm install`, you're still likely to get JavaScript/C files *that you can actually look at*, unlike this eco-friendly hairball of a thing. And regardless of whether I build it for you or you do it, the problem still exists, because I'd be doing exactly the same thing you are. I suppose I *could* release slowly audited builds signed with my PGP key and assume the legal risks of promising people that the code is safe to use. But ask yourself this question, $238723 bajillion startup faketepreneur: **are you going to pay me to do it?** Because I do a lot of things for free for people, but making your ass rich by assisting you in sucking code you barely understand into a chunk of your proprietary backend is not one of them, you special snowflake you.

* [Node.js](http://nodejs.org) is the greatest thing to ever happen to JavaScript. [Browserify](http://browserify.org) is the second greatest thing. If you're a full-time JavaScript programmer doing something important with BitcoinJS, you should probably learn how to use them.

* If this crazy-sounding rant has unnerved you about implicitly trusting pre-packaged code from me, I have accomplished my goal. Thank me when this prevents your company from turning into Mt Gox Reloaded.

## Thanks for wasting some time for me, anything else? I've got a few more minutes to waste.

[Reflections on Trusting Trust - Ken Thompson](http://cm.bell-labs.com/who/ken/trust.html)

## PCP and/or Alpaca socks fund

1Q5gek6gZc4E8dREcTkctQNtcb8dmikX1p