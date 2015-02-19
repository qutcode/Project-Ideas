# Assets Mangler

## Author
Marais Rossouw

## Required Technologies
TBA, but most lickly Node

## Project Description
So basically I have this idea to write a middle ware to once you have all your assets (JS, and CSS) built, minified etc to then go through and mangle all css selectors. Right now I have a PHP version for Laravel which you run by php ./artisan assets:mangle and it works quite well. Goes in and parses the css stylesheet's finds all selectors then mangles them with the alphabet. It counts the selectors, then finds the optiminal length of the selector. So in most cases a length of 2 charaters upper and lower case. Then parses the HTML output creates a DOM Document and recurses that string replaceing all selectors (pre_replace, just wasnt fast enough, or stable). Then caches the output for subsequent requests. My only main concern is where i am stuck is the js, where it goes and selects elements in the dom. I have it working, but then you have edge cases like filters,  finds etc.. So really wanting someone to team up and build something amazing. From what i do have, js asside, the pain time was increased by about 60ms and a way less memory footprint. Same with file sizes.

# Comments Area
Performance. See with css, the longer the nest the slower it takes to render. So i want to eventually evolve this into actually assessing the dom, and create move, and alter selectors to get those selectors down to as low as possible nesting.

See Google, Facebook, and all the large guys do it. Because they have millions of traffic a day and thus billions of transit a day so the tiniest change in speed or servability of assets might just save them terabytes of transit.

Now im not saying coz Google does it, we must do it. Obviously their scope is a lot different than the average website. But I see it as more of a challenge to get selectors mangled effectively. And frankly there is nothing out there in the open source world or paid source world that does this, now just imagine if we could actually pull this off in a npm sort of scenario and actually help improve the web as we know it.

Ultimately who wouldn't want to try and protect IP in terms of how things are done on major websites simply because we as human cannot make sense of anything selector base.

I mean come on, Google Closure Compiler did wonders to JS, why not have something similar for styles!
