/* 
1) Quick General Effects
2) Subreddit Shortcuts Bar at the top of the page
3) Header
4) Tabs
5) Genre Lists
6) Body
7) Sidebar
8) Comment page edits
9) Submission Page edits
10) Flairs
11) np CSS or antiraid stuff
*/



/* 1) Quick General Effects
############################################################################################################################################################################################*/

/*change highlights on mouse selection*/
::selection {background-color:#8676AE;color:#F0F0F0; }

/*remove footer*/
div.footer-parent{
  
    padding-top: 80px;
}
/*no bottom menus*/
.footer, .bottommenu { display: none; }

/*kills recently the recently viewed links box*/
ul.content:nth-child(2), div.title:nth-child(1) > h1:nth-child(1), .account-activity-box > p:nth-child(1)
{
  display: none;
}

/*kills the community button and shit below it like "for your WoW guild"*/
.sidebox.create .morelink
{
  display: none;
}
.sidebox.submit .spacer a, .sidebox.create .spacer a
{
  display: none;
}
.sidebox.create .morelink
{
  display: none;
}
.sidebox.submit .spacer
{
  display: none;
}
.sidebox.create .spacer
{
  display: none;
}
h1
{
  display: none;
}


/*change scroll bar looks*/
::-webkit-scrollbar {
    width: 12px;
  background: #eee;
}
/* Handle */
::-webkit-scrollbar-thumb {
    border-radius: 1px;
    background: #b3b3b3;  
}


/*modify RES never ending reddit crap*/
.NERPageMarker{
  margin-top: 0px !important;
  margin-bottom: 0px !important;
  padding: 0px 0 !important;
  color: #aaa !important;
  border: 0px solid transparent!important;
  background-color: transparent!important;
}
#progressIndicator{
  border: 0px solid #999 !important;
  border-radius: 0px !important;
  background-color: transparent !important;
}
#progressIndicator h2 {
  color: #aaa !important;
}
p.NERWidgetText{
  display:none;
}

/*remove RES last clicked border*/
.link.last-clicked
{
  border: none;
}

/*fix boxes*/
.sheets {
  margin-right: 500px;
  margin-left: -15px;
  overflow: visible;
}

/*hide pi*/
.debuginfo {
  display: none;
}

/*change RES highlight color*/
.RES-keyNav-activeElement{
  background-color: #E5EDFF;
}

.login-form-side{
  border-style: none;    

}




/* 3) Header
############################################################################################################################################################################################*/

/*user karma bar font color*/
#header-bottom-right a, .user .userkarma, .user
{
  color: #F0F0F0;

}

#header-bottom-right{
  background-color: transparent !important;
}

#RESMainGearOverlay .gearIcon
{
  display: none;
}

/*collapse button in RES user karma bar */
#userbarToggle
{
  color: #F0F0F0 !important;
  background-color: transparent !important;
  border-right: none !important;
  line-height: 26px !important;
  bottom: 1px;
}


/*RES user karma bar, main field*/
.res #header-bottom-right
{
  background: transparent;
  color: #F0F0F0 !important;
  line-height: 0em !important;

  margin: -1px 0px 0px 0px;
  border-radius: 1px;
}

/* Sub logo */
.pagename {
  font-size: 0;
}

.pagename a {
  left: 0;
  right: 0;
  top: 19px;
  bottom: 0;
  position: absolute;
  background: #111 url(%%RBER-7%%) no-repeat;
  text-indent: -9999em;
}




#header-img {
  width: 180px;
  height: 49px;
  position: absolute;
  bottom: 0;
  left: 5px;
  z-index: 1;
}



#header {
  height: 154px;
  border-bottom: 30px solid #333;
  position: relative;
  z-index: 99;
}






	





		
/*4) Tabs 
############################################################################################################################################################################################*/



/* HOT / NEW / ETC */
#header .tabmenu {
  display: block;
  position: absolute;
  top: 151px;
  right: 0px;
  left: 0px;
  padding: 3px 0px 7px 0px;
  height: 20px;
  background-color: #f5f5f5;
  border-bottom: 1px solid #DADADA;
  color: #707070;
  list-style-type: none;
  vertical-align: bottom;
  text-align: left;
  white-space: nowrap;
  font-weight: normal;
  font-size: 15px;
  font-family: Calibri, Candara, Segoe, "Times New Roman", Optima, Arial, sans-serif;
  min-width: 450px;
  bottom: 0;
  z-index: 1;
  
}

.tabmenu li {
  display: inline-block;
  margin: 0px;
}

.tabmenu li a {
  margin: 0px 20px 0px 20px;
  padding: 2px 5px 4px 5px;
  background-color: transparent;
  border: 0px solid;
  color: #737373;
  font-weight: normal;
  font-size: 20px;
  font-family: Baskerville,Candara,Segoe,"Times",Optima,Arial,sans-serif;
}

.tabmenu li a:hover {
  border-bottom: 2px solid #9b70fa;
  color: #262626;
  text-decoration: none;
}

.tabmenu li.selected a {
  z-index: 100;
  background-color: transparent;
  border: 0px solid;
  border-bottom: 2px solid #9b70fa;
  color: #262626;
  font-size: 20px;
  font-family: Baskerville,Candara,Segoe,"Times",Optima,Arial,sans-serif;
}

.tabmenu li.selected a:hover {
  border-color: #719ff2;
}

/* Message displayed under top level text box */

.commentarea .usertext .bottom-area {
  position: static;
}

.commentarea .usertext .usertext-edit .bottom-area:before {
  margin-top: 3px;
  content: "Note: We may remove personal attacks, as well as bigoted or hateful comments, including those directed towards any race, religion, ethnic group, nationality, gender, or sexual orientation. Repeat offenders may be banned.";
  display: block;
  padding: 5px;
  background-color: #a296c1;

  font-size: 12px;
  font-weight: bold;
  -webkit-border-radius: 7px;
  -moz-border-radius: 7px;
  border-radius: 0px;
}







/* 6) Body 
############################################################################################################################################################################################*/



.content {
  margin: 15px 12px 0px 12px !important;
}

/*!!!!!!!!!!important because link outlines. makes good highlight effect for RES*/
div.link {
  padding: 0px;

  overflow: hidden;
  margin: 0;
}
.entry
{
  padding: 10px 0px 10px 5px;
  border-style: none;
  border-color: transparent;
  overflow: visible;
  margin-left: 0;
}
.commentarea .entry{
  overflow: hidden;
  padding: 0px 0px 0px 5px;
}
.thumbnail{
  margin: 10px 5px 10px 0px;
  overflow: hidden;
}
.link .midcol{
  margin-top: 11px;
  margin-left: 6px;
  margin-bottom: 8px;
  margin-right: 5px;
}
.comment .midcol{
  margin-right: 0px;
}

.link .rank {
  display: none;
}

.comment.noncollapsed .midcol {
  margin-top: 9px;
}

.linklisting .odd {
   overflow: visible!important;
    margin: 0px !important;
    background-color: #f1f1f1;
    min-height: 50px !important;
}
 
.linklisting .even {
   overflow: visible!important;
    margin: 0px !important;
    background-color: #f4f4f4;
    min-height: 50px !important;
}

/* hover text for the downvote button */
.arrow.down:hover:before {
  position: absolute;
  display: block;
  z-index: 1000;
  width: 210px;
  padding: 5px;
  border: 0px solid #333;
  background: #8676ae;
  content: "Don't downvote simply because you don't agree";
  text-align: center;
  font-size: 10px;
  color: black;
  margin-left: 25px;
  margin-top: 5px;
  -moz-border-radius: 4px;
  border-radius: 4px;
  -webkit-border-radius: 4px;
}	

/* hover text for the report button */
.report-button .option:not(.error):hover:before {
  color: black;
  background-color: #def;
  border: 1px solid #333;
  border-radius: 4px;
  content: "Please report comments that violate the rules.";
  display: block;
  font-size: 9.5px;
  font-weight: bold;
  margin-left: 75px;
  margin-top: 7px;
  padding: 5px;
  position: absolute;
  text-align: center;
  z-index: 1000;
}

.link .flat-list, .link .tagline {

  overflow: hidden;
}
/*show comments button but hide the save, hide, delete, spam, remove, nsfw, [l+c] buttons  */
#siteTable div.thing ul.flat-list li a:not(.comments):not(.title)
{
  opacity: 0;
  transition: all .2s ease-out;
}
.comments-page #siteTable div.thing ul.flat-list li a:not(.comments)
{
  opacity: 1;
}
#siteTable div.thing:hover ul.flat-list li a:not(.comments):not(.title)
{
  opacity: 1;
}
/*lazy/hacky to remove l+c for RES*/
#siteTable div.thing ul.flat-list li .redditSingleClick {
  opacity: 0;
    transition: all .2s ease-out;
}
#siteTable div.thing:hover ul.flat-list li .redditSingleClick {
  opacity: 1;
}

/*modify comments button font*/
.link .entry li .comments
{
  visibility: visible;
  color: #8676AE;
  font-weight: bold;
  font-size: 11px;

}
.entry .buttons a[onclick*="reply"]
{
  color: #8676AE;
  font-size: 11px;
}

/*visited and unvisited links customization*/
.thing .title
{
  color: #222;
  font-size: 17px;
}
.thing .title:visited, .thing.visited .title
{
  color: #999;
}








/* 7) Sidebar
############################################################################################################################################################################################*/

/*side styling*/
.side {

  width: 300px;
  margin: 27px 24px 0px auto;
  padding: 10px !important;
  z-index: 0;
  border-radius:1px;
  box-shadow: 0px 1px 3px 1px #bbb;
  background: #eee6f0;
  overflow: hidden;
}

.side .md {
    overflow: hidden;
}

.side hr {
    visibility: hidden;
}



/*customize search bar*/
#search input[type=text]{
  border-style:none;
  background: #ccc6dd;
  box-shadow: 0 5px 10px -6px black;
  content: '';
  padding: 5px 0 5px 0;
  width: 299px;
}
#search input[type="text"]:-moz-placeholder { 
    font-size: 0;
    color: #fff;
}

#search input[type="text"]::-webkit-input-placeholder { 
    font-size: 0;
    color: #fff;
}

#search input[type="text"]:-moz-placeholder::after {
    font-size: 15.4px;
    content: "Search";
    font-family:  verdana,arial,helvetica,sans-serif;

    letter-spacing: -1px;
    line-height: 20px;
    font-weight: 700;
}

#search input[type="text"]::-webkit-input-placeholder::after {
    font-size: 15.4px;
    content: "Search";
    font-family:  verdana,arial,helvetica,sans-serif;

    letter-spacing: -1px;
    line-height: 20px;
    font-weight: 700;
    
}
input[placeholder] {
    text-align: center;
}

/*change search popup location*/
#searchexpando {
  position:absolute;
  right: 360px;
  width: 279px;
  margin-top: -31px !important;
  border: 0px solid transparent ;
  border-radius:1px;
  background:#CCC6DD;
  z-index:99;
}




/*get rid of nub in submit buttons*/
.morelink .nub
{
  display: none;
}

/* Submit :Link */
/* Updated to conform to CSS standards */
/* Padding below Submit Link .titlebox { padding-top: 49px; }*/

/*Chatroom button: Activate by uncommenting */
.side .md a[href="https://carrot.com/r/economics"] {
    text-transform: none;
    display: block;
    border: none;
    color: #FFF!important;
    position: relative;
    text-align: center;
    text-transform: none;
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    border: 1px solid #C16200;
    box-shadow: inset 0 1px 2px rgba(255, 255, 255, 0.3), 0 1px 2px rgba(19, 49, 69, 0.2);
    letter-spacing: 0px;
    border-radius: 4px;
    border: 1px solid #C16200;
    font-size: 17px;
    font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen,Ubuntu,Cantarell,"Open Sans","Helvetica Neue",sans-serif;
    line-height: 39px;
    text-decoration: none;
    height: 38px;
    background: -webkit-linear-gradient(top, #72b94c, #1ba41b);
    background: linear-gradient(to bottom,#72b94c, #1ba41b);
}

.side .md a[href^="https://carrot.com/r/economics"]:hover {
    background: -webkit-linear-gradient(top, #EF800D, #FE8D2C);
    background: linear-gradient(to bottom, #EF800D, #FE8D2C);
    -webkit-transition: all .2s;
    transition: all .2s;
}

.side .md a[href^="https://carrot.com/r/economics"]:active {
    background: -webkit-linear-gradient(top,#d3721f,#ff9c36);
    background: linear-gradient(to bottom,#d3721f,#ff9c36);
    box-shadow: inset 0px 0px 0px 0px rgb(0,0,0) !important;

}

/* button icon */

.side .md a[href^="http://carrot.com/r/economics"] {
    background-image: url(%%buttonicon%%);
    width: 100px;
    height: 100px;
    border-radius: 3px;
    top: 29px;
    left: 41px;
    position: relative;
    border: 1px solid rgba(0, 0, 0, 0.55);
    z-index: 30;
    background-position: center center;
    background-size: 100% auto;
    background-repeat: no-repeat;
}


.morelink a[href="https://www.reddit.com/r/Economics/submit"] {
color: #fff;
}

.side .submit-link .morelink {
    display: block;
    margin-bottom: 15px;
    border: none;
    color: #FFF !important;
    text-align: center;
    text-transform: capitalize;
    text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    box-shadow: inset 0 1px 2px rgba(255, 255, 255, 0.3), 0 1px 2px rgba(19, 49, 69, 0.2);
    letter-spacing: 0px;
    border-radius: 4px;
    border: 1px solid #000000;
    font-weight: bold;
    font-size: 17px;
    line-height: 42px;
    text-decoration: none;
font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen,Ubuntu,Cantarell,"Open Sans","Helvetica Neue",sans-serif;
    height: 41px;
    background: -webkit-linear-gradient(top, #4c4c4c, #000000);
    background: linear-gradient(to bottom, #4c4c4c, #000000);
}

.side .submit-link .morelink:hover {
    background: -webkit-linear-gradient(top, #686868, #282828);
    background: linear-gradient(to bottom, #686868, #282828);
    -webkit-transition: all .4s;
            transition: all .4s;
    cursor: pointer;
}

.side .submit-link .morelink:active {
    background: -webkit-linear-gradient(top, #2e2e2e, #2e2e2e);
    background: linear-gradient(to bottom, #2e2e2e, #2e2e2e);
    box-shadow: none;
    color: #b4b4b4 !important;
    cursor: pointer;
}


/*format submit text*/
.side .submit-text .morelink
{
  background-image: none;
  background: hsl(260,25.3%,62.7%) !important;
  border: none;
  font-size: 0;
  padding-top: 2px;
  border-bottom: 3px solid hsl(259.3, 24.8%,55.7%) !important;
  border-radius: 1.5px;
  box-shadow: 0px 1px 1px rgba(88,88,88,.84);
  display: none;
}

.side .submit-text .morelink a:after
{
  content: "Submit a Text Post";
  font-size: 15px;
  color: #F0F0F0 !important;
  transition: all .3s ease;
}

/*weird bug fix related to above*/
.submit.mod-override .morelink a:after{
  position: relative;
  background: none;

}


/*change reading now icon*/
.users-online:before{
  background: #8676AE;
  border-radius: 3px;
}


/*remove leave moderator box in sidebar*/
.titlebox form.toggle, .leavemoderator
{
  display: none;
}

/*center RES use subreddit style*/
.side .redditname + div {
    text-align: center;
}




/*fuck all this RES BS*/
.subscribe-button .option.active {
    display: inline-block;
}

.res .RESshortcutside,
.res .RESDashboardToggle {
  
    margin: 0 0 0 .5em;
    width: auto;
    border-radius: 0;
    line-height: 1.2;
    vertical-align: top;
    display: inline-block!important;
}
#subButtons-economics .subscribe-button a {
    font-size: .9em;
    border-radius: 0;
}
.res .RESshortcutside,
.res .RESDashboardToggle {
    font-size: .9em;
}
.res .side .subscribe-button,
.res .side .RESshortcutside,
.res .side .RESDashboardToggle {
    width: 33%;
    margin-left: 0;
    margin-right: 0;
    text-align: center;
    padding: .3em 0;
    border: 0;
  
}
.res .side .subscribe-button {
    padding: 0;

}
.res .side .subscribe-button .option {
    width: 100% !important;
    padding: 0 0 0 0 !important;
    vertical-align: top;
    border: 0 !important;
    height:19px;
    border-radius: 0;
}
.side .subscribe-button .add:before {
    content: '+'
}
.side .subscribe-button .remove:before {
    content: '-';
}
.side .subscribe-button .add {
    background: red;
  border-style: none;
  border-radius: 0;
}

.side .subscribe-button .remove {
    background: #CCC6DD;
  border-style: none;
  border-radius: 0;
}

.res .side .RESshortcutside {
    background: #CCC6DD;
    width: 34%;
}

.res .side .RESDashboardToggle {
    background: #CCC6DD;
}




/*static rules top bar*/
.side .md h2 {
box-shadow: 0px 1px 1px rgba(88,88,88,.84);
  padding: 3px 0;
  text-align: center;
  width: 300px;
  color: #FFF!important;
  /*letter-spacing: 1px;*/
  text-transform: capitalize;
  font-weight: normal!important;
  display: block;
  font-size: 16px;
  background: #beb6d3;


  border-radius: 1.5px;
}
/*static rules drop down*/
.side .md h2+blockquote {
box-shadow: 0px 1px 1px rgba(88,88,88,.84);
text-align: center;
  width: 290px;
  display: block;
  background-color: #CCC6DD;
  border: 0;
  color: #000!important;
  margin: 0px 0px 5px 0px;
  padding: 2px 5px 2px 5px;
  border-radius: 1.5px;
box-shadow: 0 5px 10px -6px black;
}


/*Subreddit Rules bar*/
.side .md h3 {

  padding: 3px 0;
  text-align: center;
  width: 300px;
  color: #000!important;
  /*letter-spacing: 1px;*/
  text-transform: capitalize;
  font-weight: normal!important;
  display: block;
  font-size: 16px;
  background: #aecaa6;


  border-radius: 1.5px;
}
.side .usertext-body ol {
box-shadow: 0px 1px 1px rgba(88,88,88,.84);
    list-style-type: upper-roman !important;

    padding-left: 32px;
    width: 250px;
    overflow: hidden;

    border-color: #BFE1FF !important;
    padding-right: 19px;

    
  margin: 0px 1px 0px 0px;
    background-color: #cbddc6 !important;
    box-shadow: 0 5px 10px -6px black;
    
    
}

.side .titlebox .usertext-body ol ol{
box-shadow: 0px 1px 1px rgba(88,88,88,.84);
    list-style-type: lower-roman !important;
    margin-top: -2px;
    margin-left: 0px !important;
    color:black !important;
    font-size:100%;
    box-shadow: none !Important;
    width: 198px;
    padding-right: 10px !important;
    border: none !important;
    
    
    text-align: left !important;
}


.titlebox .bottom , .sidecontentbox .content {
  border-style:none;
  padding: 0;
  margin: 4px 5px 0px 7px !important;
}

/* edit created by */
.side .bottom { font-size: 0; content: ''; position: relative; }
.side .bottom .age { font-size: x-small; }
.side .bottom .age:before {
  content: 'CSS by Phinaeus';
  position: absolute;
  left: 0;
  margin-left: -7px;
}

###################################################################################
/* 7.1) mberre edit march 2015


.listing-page .side > .spacer:first-child,
.comments-page .side > .spacer:first-child,
.search-page .side > .spacer:first-child {
    padding-top: 110px;
}
.sidebox.submit {
    position: absolute;
    top: 220px;
    right: 35px;
    width: 300px;
}
.side .md [href$="/r/Economics/wiki/reading"] {
    position: absolute;
    height: 45px;
    width: 300px;
    right: 35px;
    background: url(%%reading-list-button%%);
    top: -9999em;
}
.listing-page .side .md [href$="/r/Economics/wiki/reading"],
.comments-page .side .md [href$="/r/Economics/wiki/reading"],
.search-page .side .md [href$="/r/Economics/wiki/reading"] {
    top: 280px;
}




#####################################################################################
/* 8) Comment page edits
############################################################################################################################################################################################*/

/*modify border around res comments*/
.res-commentBoxes .comment {

  border-bottom: 0px solid #ddd !important;
  border-right: 0px solid #ddd !important;
  border-top: 1px solid #f5f5f5 !important;
  border-left: 2px solid #ddd !important;
  border-radius: 0px !important;
  margin-bottom: 5px !important;
}

.link .usertext .md{
    
  border: 1px solid #BEB6D3;    
  border-radius: 2px;
}

.panestack-title{
  border-style:none;    

}

.linkinfo{
  border-style:none;    
  background-color: #CCC6DD;    
  box-shadow: 0 5px 10px -6px black;
  border-radius: 0;
}



/*10) Flair
############################################################################################################################################################################################*/

.flair-QC {
  background: #8576AD !important;
  color: white !important;

    
}


/* 11) np CSS or antiraid stuff
############################################################################################################################################################################################*/

/* ------------------------- */
/* BEGIN COPY */



/* "No Participation"-Mode, aka "Read Only"-Mode
 * by /u/KortoloB
 * /r/NoParticipation
 * 
 * Link people to np.reddit.com/r/YourSubreddit to show them a read-only version.
 * Subscribers will see the full page, only non-subscribers will see the read-only version.
 * This is of course by no means fool-proof, but it should work for the average user.
 *  */

body:lang(np):not(.subscriber) .arrow
{ 
    visibility: hidden !important;
}

body:lang(np):not(.subscriber) .usertext-edit,
body:lang(np):not(.subscriber) .sidebox.submit,
body:lang(np):not(.subscriber) .commentingAs,
body:lang(np):not(.subscriber) .markdownEditor, 
body:lang(np):not(.subscriber) a[onclick*="return reply(this)"],
body:lang(np):not(.subscriber) .subButtons,
body:lang(np):not(.subscriber) .helplink,
body:lang(np):not(.subscriber) .titlebox .fancy-toggle-button.toggle > .option.add
{
    display: none !important;
}

body:lang(np):not(.subscriber) #siteTable:before
{
    content: "You have been linked to a read-only version of this subreddit. Please respect the community by not voting.";
    display: block;
    max-width: 800px;
    background-color: #F6E69F;
    padding: 5px 10px;
    margin: 5px 305px 5px 0px;
    border: 1px solid orange;
    font-size: small;
}

body:lang(np):not(.subscriber) .entry.likes:not(.reddit-entry):before,
body:lang(np):not(.subscriber) .entry.dislikes:not(.reddit-entry):before
{
    content: "Please do not vote or comment when you come from external subreddits.";
    color: red;
    font-size: large;
    font-weight: bold;
}

/* Wiki protection */
body.wiki-page:lang(np):not(.subscriber) span.pageactions a.wikiaction-edit:not(.wikiaction-current),
body.wiki-page:lang(np):not(.subscriber) div.wiki-page-content form#editform label[for='reason'],
body.wiki-page:lang(np):not(.subscriber) div.wiki-page-content form#editform input#wiki_revision_reason,
body.wiki-page:lang(np):not(.subscriber) div.wiki-page-content form#editform input[type='submit']
{
    display: none !important;
}



/* END COPY */
/* ------------------------- */
