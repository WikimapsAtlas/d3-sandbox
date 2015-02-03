### D3-sandbox

> _"Demo it or it doesn't exist."_
> -- The hacker manifesto

<!--
#### V.1.0
This repository was the former d3js sandbox / demobox of the Wikimaps Atlas project. 
We here use geojson or topojson data from the Wikimaps Atlas API, beautifying them using D3js.
When one visualisation type is mature, we integrage the code into our map generator system, 
loop all over the world, so all areas are displayed elegantly with this style.

#### V.2.0
We now recommand dev-cartographers to [create][1] and demo **stand alone gists**, with relevant css & js.
Your gists create your own porfolio publicly visible via Mike Bostock's [Bl.ocks.org][2] service.

You can then submit us your link on our issue page. 
We welcome it, will add your gist url and description to the list of D3js cartographic gists.
The most interesting visualisation for encyclopedic usages will be integrated
into Wikipedia's Wikimaps project to map all countries of the world with it :)
-->
### Structure

 - `./index.html` is the central page which should diplays maps
 - `./js/wikiatlas.js` personal library to draw each king of map.
 - `./js/` contains convenient js files
 - `./x.y_folder` , numbers indicate both priority & maturity (1.1 > 2)
 - `./data/` contains old data for D3js community
 - `./output/` contains new data sample from make-module

#### Contacts

* @hugo_lz (Hugo Lopez)
* @planemad (Arun Ganesh)

### Lighten repository
Use wisely, notify your teammate.

```
git config --get remote.origin.url
rm -rf .git
git remote rm origin
git init
git add .
git commit -m "Initial commit"
git remote add origin git@github.com:WikimapsAtlas/d3-sandbox.git
git push -u --force origin master
```

[1]: https://gist.github.com/new
[2]: http://bl.ocks.org


