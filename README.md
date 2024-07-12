# liz nichols portfolio website
--
Hello. Here are some notes about the files above.

1. index.html is the main site code. it has all the website text and image files and basic HTML structure. most website hosting sites will recognize index.html as the main / home page of a site and will by default render it at the root domain

2. site.css and static.css are stripped from squarespace and just saved locally so there's no more style dependency. they are minified and ugly and i recommend just leaving them as they are.

3. thenewstuff.css is my new CSS file with my own custom styles. this was needed to replicate mainly to replicate the image grid experience outside of squarespace. i cut any JS dependencies and without them, the grid kinda crashed. this thenewstuff.css fixes it back up again. this is the file we'll edit if new styles are needed on site. 

4. site-bundles.js is actually unneeded. it's here when i tried stripping the JS files to render locally, but it didn't work. and honestly it just isn't needed. your site doesn't require JS right now, and if it does in the future, we'll just start from scratch.
