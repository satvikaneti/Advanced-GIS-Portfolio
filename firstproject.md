# Creating a Google Maps Base Layer

For this project, I chose the nonprofit [AAPI Data](https://aapidata.com/). I really respect the work this organization is doing, in gathering and working to disaggregate the data of the distinct AAPI communities. When I checked their website, I saw that they had a pretty consistent color palette of yellows, oranges, and greys, with a hint of pink here and there. I wanted to re-create that in my map. Using a color picker extension on Chrome and Canva's color palette tool, I created this palette of colors I wanted to use for the base map:

![image](https://user-images.githubusercontent.com/59181449/112777824-208eb800-9011-11eb-864b-5329a039dc6d.png)

I played around with the different colors - I knew I wanted the grey and black to take up most of the background, just as in the website, and I knew I wanted the pink to be more of a highlight color. Getting the water color down was the tricky bit - I experimented with bright colors like the yellow or the pink for the waterways, but when zoomed out to a world view it just made the world look like it was on fire, so I ended going witht the dark black for water and the lighter grey for most of the rest of the background. 

The roads I always knew I wanted to be that golden color, so then picking the parks colors and transit colors stemmed from that. At first I had both be pink, but that ended up being too much pink, and it was too disconnected from each other (parks and transit are _somewhat_ connected, but not enough that they should be portrayed as the same on a map). So then I switched to the darker orange for the parks, which turned out to be a good decision. The orange looked similar enough to the gold to not be obtrusive, but not so similar that they blended into each other. Transit then became pink, which worked out for the highlight view I was going with for with that color. I also ended up upping the weights on the transit lines so they would pop more, which also heightened that effect.

For the text, I tried both the yellow and the pink. The pink was way too obtrusive, and ended up almost taking over the map. The yellow worked nicely with the rest of the background while still standing out by itself. It also is the color that's used for most of the big text on the website, so it makes sense for that reason also. 

Here's the final map: 

<iframe src="https://satvikaneti.github.io/Advanced-GIS-Portfolio/gmapfirstproj.html" width="100%" height="800px"></iframe>
