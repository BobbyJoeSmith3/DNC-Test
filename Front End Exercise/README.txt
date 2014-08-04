Hello!

Most of everything I wanted to communicate with you is already embedded in the code in the form of comments, but I wanted to add a few points as well.

First, instead of having all of the scripts and images in one folder along with the images, and instead of inline styling the html, I chose to modularized the html, css, and images into two folders -- static and templates. The paths written into the code are localized to my computer. In order to see the styling and have the images show up on the screen, you will need to write your own links with the appropriate path to the content.

Second, I didn't have the time to insert the functionality of the website and debug it, but this is how I would have approached it conceptually. 

In order to have the user navigate through the site without directing them to new pages, I would have used the jQuery javascript library to hide and show content as necessary. When a user clicks on one of the "navpoints" in the navigation bar, the navpoint marker which was previously hidden would show, and the other two would be hidden (this is why in the sample I am sending you, all of the navmarkers are displayed on each of the navpoints). Similarly, the content pertaining to that page would show, and the content for the other two unselected navpoints would be hidden. In reality, all of the content is on the same page at the same time, but by using the hide/show effect in jQuery, we can make it appear as if only the appropriate information is on the page at one time. The code would look something to the effect:


$("#hide").click(function(){
  $("p").hide();
});

$("#show").click(function(){
  $("p").show();
});


The other option that might work would be using a slide effect. When a user clicks on a navpoint in the navbar, the previous copy that was being displayed would slide to the side (closing in a way that we are used to seeing with dropdown menus) and the the copy that correlates to the page would slide out onto the screen. We would still use the hide/show effect for the navmarkers. This effect is also done through jQuery.

That is all, if you need any other clarification, feel free to contact me at bobbyjoe@codeforprogress.org

Best,
Bobby Joe

