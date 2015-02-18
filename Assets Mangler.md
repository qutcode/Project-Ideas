# Assets Mangler

## Author
Marais Rossouw

## Required Technologies
TBA, but most lickly Node

## Project Description
So basically I have this idea to write a middle ware to once you have all your assets (JS, and CSS) built, minified etc to then go through and mangle all css selectors. Right now I have a PHP version for Laravel which you run by php ./artisan assets:mangle and it works quite well. Goes in and parses the css stylesheet's finds all selectors then mangles them with the alphabet. It counts the selectors, then finds the optiminal length of the selector. So in most cases a length of 2 charaters upper and lower case. Then parses the HTML output creates a DOM Document and recurses that string replaceing all selectors (pre_replace, just wasnt fast enough, or stable). Then caches the output for subsequent requests. My only main concern is where i am stuck is the js, where it goes and selects elements in the dom. I have it working, but then you have edge cases like filters,  finds etc.. So really wanting someone to team up and build something amazing. From what i do have, js asside, the pain time was increased by about 60ms and a way less memory footprint. Same with file sizes.

# Comments Area
Hope any of this makes sense
