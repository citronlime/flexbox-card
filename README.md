# flexbox-card
Flexbox-project
1. Placing a card in the center of the screen both horizontally and vertically setting display:flex on the body and using min-height:100vh to be able to set align-items:center and justify-content:center
When doing this the container for  the card should no hava margin:0 auto set
2. Also trying flex-basis to have an image to be displayed to the left on larger screens and at the top on a small screen with column layout. There is a fix to handle that the image looses its size when using flex basis.
The trick is to add  min-width: 0; min-height: 0; to the image class and flex-basis: 200px that will be the height in a column direction(the mobile) and the width in a row(larger screen) direction, flex-basis is applied to the main-axis
So then if you make a media query to apply to larger screens you set the height:300px(or whatever) for the image in a row mode, the width will be the flex-basis width of 200px If min-width is set on the item it will prevent the flex-basis of kicking in
