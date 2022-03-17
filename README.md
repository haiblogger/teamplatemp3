# teamplatemp3

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE html>
<html b:css='false' b:defaultwidgetversion='2' b:layoutsVersion='3' b:responsive='true' b:templateVersion='1.3.0' expr:class='data:blog.languageDirection' expr:dir='data:blog.languageDirection' expr:lang='data:blog.localeUnderscoreDelimited' xmlns='http://www.w3.org/1999/xhtml' xmlns:b='http://www.google.com/2005/gml/b' xmlns:data='http://www.google.com/2005/gml/data' xmlns:expr='http://www.google.com/2005/gml/expr'>
<b:include name='theme-dark-mode'/>
<head>
<b:include name='theme-head'/>
<b:if cond='data:blog.pageType == &quot;item&quot;'>
 <script src="https://raw.githack.com/o0okokojumbo/audiotruyenvn/master/jquery.min.js" type="text/javascript"></script>
</b:if>
<b:if cond='!data:view.isLayoutMode'>
<!-- Theme CSS Style -->
<b:skin version='1.3.0'><![CDATA[

/* -----------------------------------------------
Blogger Template Style
Name     :  Doc Truyen Online
License  :  Premium Version
Version  :  v1.0.0
Author   :  Jack
----------------------------------------------- */

/*
<!-- Variable definitions -->
<Variable name="keycolor" description="Main Color" type="color" default="#1A73E8" value="#1A73E8"/>
<Group description="Theme Options">
    <Variable name="darkmode" description="Native Dark Mode" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="userdarkmode" description="User Dark Mode" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="fixedmenu" description="Fixed Menu" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="sidebar" description="Left Sidebar" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="fixedsidebar" description="Fixed Sidebar" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Widths">
    <Variable name="boxed" description="Boxed Mode" type="length" default="0px" min="0px" max="1px" value="0px"/>
    <Variable name="row.width" description="Container Width" type="length" default="1170px" min="1000px" max="1170px" value="1170px"/>
    <Variable name="sidebar.width" description="Sidebar Width" type="length" default="330px" min="280px" max="350px" value="330px"/>
</Group>
<Group description="Theme Fonts">
    <Variable name="main.font" description="Site Font" type="font" family="Verdana" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="menu.font" description="Menu Font" type="font" family="Verdana" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="title.font" description="Title Font" type="font" family="Verdana" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
    <Variable name="text.font" description="Text Font" type="font" family="Verdana" default="normal 400 14px $(family)" value="normal 400 14px $(family)"/>
</Group>
<Group description="Background">
    <Variable name="background.color" description="Body Background" type="color" default="#F1F3F4"  value="#F1F3F4"/>
    <Variable name="body.background" description="Background" type="background" color="$(background.color)" default="$(color) none repeat fixed top left" value="$(color) none repeat fixed top left"/>
    <Variable name="outer.bg" description="Outer Background" type="color" default="#FFFFFF"  value="#FFFFFF"/>
    <Variable name="outer.mobile.bg" description="Outer Mobile Background" type="color" default="#F1F3F4"  value="#F1F3F4"/>
</Group>
<Group description="Theme Colors">
    <Variable name="main.color" description="Theme Color" type="color" default="#1A73E8" value="#1A73E8"/>
    <Variable name="title.color" description="Title Color" type="color" default="#202124" value="#202124"/>
    <Variable name="title.hover.color" description="Title Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
    <Variable name="meta.color" description="Meta Color" type="color" default="#636466" value="#636466"/>
    <Variable name="text.color" description="Text Color" type="color" default="#3C4043"  value="#3C4043"/>
</Group>
<Group description="Site Header" selector="#header-wrapper">
    <Variable name="header.bg" description="Header Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="header.color" description="Header Color" type="color" default="$(title.color)" value="#202124"/>
    <Variable name="header.hover.color" description="Header Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="Sub Menu">
    <Variable name="submenu.bg" description="Sub Menu Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="submenu.color" description="Sub Menu Color" type="color" default="$(title.color)" value="#202124"/>
    <Variable name="submenu.hover.color" description="Sub Menu Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="Mega Menu">
    <Variable name="megamenu.bg" description="Mega Menu Background" type="color" default="$(submenu.bg)" value="#FFFFFF"/>
    <Variable name="megamenu.color" description="Mega Menu Color" type="color" default="$(submenu.color)" value="#202124"/>
    <Variable name="megamenu.hover.color" description="MegaMenu Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="Mobile Menu">
    <Variable name="mmenu.bg" description="Mobile Menu Background" type="color" default="$(outer.bg)" value="#FFFFFF"/>
    <Variable name="mmenu.color" description="Mobile Menu Color" type="color" default="$(title.color)" value="#202124"/>
    <Variable name="mmenu.hover.color" description="Mobile Menu Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="Header ADS" selector="#header-ads-wrap">
    <Variable name="headerad.onpost" description="Show on Post Page" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Widgets" select="#sidebar">
    <Variable name="widget.bg" description="Widget Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="wtitle.color" description="Widget Title Color" type="color" default="$(title.color)" value="#202124"/>
</Group>
<Group description="Post Styles" select="#main">
    <Variable name="post.title.color" description="Post Title Color" type="color" default="$(title.color)" value="#202124"/>
    <Variable name="post.title.hover.color" description="Post Title Hover Color" type="color" default="$(title.hover.color)" value="#1A73E8"/>
    <Variable name="post.text.color" description="Post Page Text Color" type="color" default="$(text.color)" value="#3C4043"/>
    <Variable name="itempost.title.size" description="Post Page Title Font Size" type="length" default="26px" min="20px" max="50px" value="26px"/>
    <Variable name="itempost.content.size" description="Post Page Text Font Size" type="length" default="16px" min="12px" max="20px" value="16px"/>
</Group>
<Group description="Post Page Options" select="#main">
    <Variable name="breadcrumb" description="Post Breadcrumbs" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="cmm.count" description="Comments Count" type="length" default="1px" min="0px" max="1px" value="1px"/>
    <Variable name="postnav" description="Post Navigation" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Footer ADS" selector="#footer-ads-wrap">
    <Variable name="footerad.onpost" description="Show on Post Page" type="length" default="1px" min="0px" max="1px" value="1px"/>
</Group>
<Group description="Theme Footer" selector="#footer-wrapper">
    <Variable name="footer.bg" description="Footer Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="footer.color" description="Footer Color" type="color" default="$(text.color)" value="#3C4043"/>
    <Variable name="footer.hover.color" description="Footer Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="FooterBar" selector=".footerbar">
    <Variable name="footerbar.bg" description="FooterBar Background" type="color" default="$(footer.bg)" value="#FFFFFF"/>
    <Variable name="footerbar.color" description="FooterBar Color" type="color" default="$(title.color)" value="#202124"/>
    <Variable name="footerbar.hover.color" description="FooterBar Hover Color" type="color" default="$(main.color)" value="#1A73E8"/>
</Group>
<Group description="Cookie Consent" selector="#gnews-pro-cookie-ify">
    <Variable name="cookie.bg" description="Cookie Background" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="cookie.color" description="Cookie Text Color" type="color" default="$(text.color)" value="#3C4043"/>
</Group>
<Group description="Theme Buttons">
    <Variable name="button.bg" description="Button Background" type="color" default="$(main.color)" value="#1A73E8"/>
    <Variable name="button.color" description="Button Color" type="color" default="#FFFFFF" value="#FFFFFF"/>
    <Variable name="button.hover.bg" description="Button Hover Background" type="color" default="#1767D0" value="#1767D0"/>
    <Variable name="button.hover.color" description="Button Hover Color" type="color" default="#FFFFFF" value="#FFFFFF"/>
</Group>
<Group description="Theme Fonts (Reset)">
    <!-- Site Font -->
    <Variable name="mainfont.italic" description="Main Font Italic" type="font" default="italic 400 14px $(main.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="mainfont.medium" description="Main Font Medium" type="font" default="normal 500 14px $(main.font.family)" value="normal 500 14px $(family)"/>
    <Variable name="mainfont.mediumitalic" description="Main Font Medium Italic" type="font" default="italic 500 14px $(main.font.family)" value="italic 500 14px $(family)"/>
    <Variable name="mainfont.bold" description="Main Font Bold" type="font" default="normal 700 14px $(main.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="mainfont.bolditalic" description="Main Font Bold Italic" type="font" default="italic 700 14px $(main.font.family)" value="italic 700 14px $(family)"/>
    <!-- Menu Font -->
    <Variable name="menufont.italic" description="Menu Font Italic" type="font" default="italic 400 14px $(menu.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="menufont.sb" description="Menu Font SemiBold" type="font" default="normal 600 14px $(menu.font.family)" value="normal 600 14px $(family)"/>
    <Variable name="menufont.sbitalic" description="Menu Font SemiBold Italic" type="font" default="italic 600 14px $(menu.font.family)" value="italic 600 14px $(family)"/>
    <Variable name="menufont.bold" description="Menu Font Bold" type="font" default="normal 700 14px $(menu.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="menufont.bolditalic" description="Menu Font Bold Italic" type="font" default="italic 700 14px $(menu.font.family)" value="italic 700 14px $(family)"/>
    <!-- Title Font -->
    <Variable name="titlefont.italic" description="Title Font Italic" type="font" default="italic 400 14px $(title.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="titlefont.sb" description="Title Font SemiBold" type="font" default="normal 600 14px $(title.font.family)" value="normal 600 14px $(family)"/>
    <Variable name="titlefont.sbitalic" description="Title Font SemiBold Italic" type="font" default="italic 600 14px $(title.font.family)" value="italic 600 14px $(family)"/>
    <Variable name="titlefont.bold" description="Title Font Bold" type="font" default="normal 700 14px $(title.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="titlefont.bolditalic" description="Title Font Bold Italic" type="font" default="italic 700 14px $(title.font.family)" value="italic 700 14px $(family)"/>
    <!-- Text Font -->
    <Variable name="textfont.italic" description="Text Font Italic" type="font" default="italic 400 14px $(text.font.family)" value="italic 400 14px $(family)"/>
    <Variable name="textfont.medium" description="Text Font Medium" type="font" default="normal 500 14px $(text.font.family)" value="normal 500 14px $(family)"/>
    <Variable name="textfont.mediumitalic" description="Text Font Medium Italic" type="font" default="italic 500 14px $(text.font.family)" value="italic 500 14px $(family)"/>
    <Variable name="textfont.bold" description="Text Font Bold" type="font" default="normal 700 14px $(text.font.family)" value="normal 700 14px $(family)"/>
    <Variable name="textfont.bolditalic" description="Text Font Bold Italic" type="font" default="italic 700 14px $(text.font.family)" value="italic 700 14px $(family)"/>
</Group>
<!-- Hidden Variables -->
<Variable name="body.background.color" description="Comments Background" hideEditor="true" type="color" default="transparent"  value="transparent"/>
<Variable name="body.title.color" description="Comments Color" hideEditor="true" type="color" default="$(title.color)" value="#202124"/>
<Variable name="body.text.color" description="Comments Text Color" hideEditor="true" type="color" default="$(text.color)"  value="#3C4043"/>
<Variable name="body.link.color" description="Comments Link Color" hideEditor="true" type="color" default="$(main.color)"  value="#1A73E8"/>
<Variable name="body.text.font" description="Comments Font 1" hideEditor="true" type="font" default="normal 400 14px Verdana, Arial, sans-serif !important"  value="normal 400 14px Verdana, Arial, sans-serif !important"/>
<Variable name="body.action.font.large" description="Comments Font 2" hideEditor="true" type="font" default="normal 700 14px Verdana, Arial, sans-serif !important"  value="normal 700 14px Verdana, Arial, sans-serif !important"/>
*/

/*-- Font Awesome Free 5.15.2 --*/
@font-face{font-family:"Font Awesome 5 Brands";font-display:swap;font-style:normal;font-weight:400;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-brands-400.svg#fontawesome) format("svg")}.fab{font-family:"Font Awesome 5 Brands";font-weight:400}
@font-face{font-family:"Font Awesome 5 Free";font-display:swap;font-style:normal;font-weight:400;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-regular-400.svg#fontawesome) format("svg")}.far{font-family:"Font Awesome 5 Free";font-weight:400}
@font-face{font-family:"Font Awesome 5 Free";font-display:swap;font-style:normal;font-weight:900;font-display:block;src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.eot);src:url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.eot?#iefix) format("embedded-opentype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.woff2) format("woff2"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.woff) format("woff"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.ttf) format("truetype"),url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/webfonts/fa-solid-900.svg#fontawesome) format("svg")}.fa,.far,.fas{font-family:"Font Awesome 5 Free"}.fa,.fas{font-weight:900}

/*-- CSS Variables --*/
:root{
--body-font:'$(main.font.family)', Arial, sans-serif;
--menu-font:'$(menu.font.family)', Arial, sans-serif;
--title-font:'$(title.font.family)', Arial, sans-serif;
--text-font:'$(text.font.family)', Arial, sans-serif;
--body-bg-color:$(background.color);
--body-bg:$(body.background);
--outer-bg:$(outer.bg);
--outer-mobile-bg:$(outer.mobile.bg);
--main-color:$(main.color);
--title-color:$(title.color);
--title-hover-color:$(title.hover.color);
--meta-color:$(meta.color);
--text-color:$(text.color);
--header-bg:$(header.bg);
--header-color:$(header.color);
--header-hover-color:$(header.hover.color);
--submenu-bg:$(submenu.bg);
--submenu-color:$(submenu.color);
--submenu-hover-color:$(submenu.hover.color);
--megamenu-bg:$(megamenu.bg);
--megamenu-color:$(megamenu.color);
--megamenu-hover-color:$(megamenu.hover.color);
--mobilemenu-bg:$(mmenu.bg);
--mobilemenu-color:$(mmenu.color);
--mobilemenu-hover-color:$(mmenu.hover.color);
--widget-bg:$(widget.bg);
--widget-title-color:$(wtitle.color);
--post-card-bg:$(widget.bg);
--post-title-color:$(post.title.color);
--post-title-hover-color:$(post.title.hover.color);
--post-text-color:$(post.text.color);
--footer-bg:$(footer.bg);
--footer-color:$(footer.color);
--footer-hover-color:$(footer.hover.color);
--footerbar-bg:$(footerbar.bg);
--footerbar-color:$(footerbar.color);
--footerbar-hover-color:$(footerbar.hover.color);
--cookie-bg:$(cookie.bg);
--cookie-color:$(cookie.color);
--button-bg:$(button.bg);
--button-lite-bg:$(button.bg)10;
--button-color:$(button.color);
--button-hover-bg:$(button.hover.bg);
--button-hover-color:$(button.hover.color);
--rgba-gray:rgba(155,170,175,0.12);
--border-color:rgba(155,155,155,0.15);
--radius:4px;
--widget-shadow:0 1px 2px rgba(0,0,0,0.025);
--avatar-shadow:0px 1px 4px rgba(0,0,0,0.05);
}
html.is-dark{
--body-bg-color:#2b2b2b;
--body-bg:#F1F3F4 none repeat fixed top left;
--outer-bg:#1a1a1a;
--outer-mobile-bg:#1a1a1a;
--title-color:#f6f7f8;
--title-hover-color:#1A73E8;
--meta-color:#aaaaaa;
--text-color:#b4b6ba;
--header-bg:#202020;
--header-color:#f6f7f8;
--header-hover-color:#1A73E8;
--submenu-bg:#252525;
--submenu-color:#f6f7f8;
--submenu-hover-color:#1A73E8;
--megamenu-bg:#252525;
--megamenu-color:#f6f7f8;
--megamenu-hover-color:#1A73E8;
--mobilemenu-bg:#1b1b1b;
--mobilemenu-color:#f6f7f8;
--mobilemenu-hover-color:#1A73E8;
--widget-bg:#202020;
--widget-title-color:#f6f7f8;
--post-card-bg:#202020;
--post-title-color:#f6f7f8;
--post-title-hover-color:#1A73E8;
--post-text-color:#b4b6ba;
--footer-bg:#202020;
--footer-color:#b4b6ba;
--footer-hover-color:#1A73E8;
--footerbar-bg:#202020;
--footerbar-color:#f6f7f8;
--footerbar-hover-color:#1A73E8;
--cookie-bg:#202020;
--cookie-color:#b4b6ba;
--button-bg:#1A73E8;
--button-color:#ffffff;
--button-hover-bg:#1767D0;
--button-hover-color:#FFFFFF;
--rgba-gray:rgba(155,155,155,0.04);
--border-color:rgba(155,155,155,0.03);
}
html.rtl{
--body-font:'Tajawal',Arial,sans-serif;
--menu-font:'Tajawal',Arial,sans-serif;
--title-font:'Tajawal',Arial,sans-serif;
--text-font:'Tajawal',Arial,sans-serif;
}
/*-- Reset CSS --*/
a,abbr,acronym,address,applet,b,big,blockquote,body,caption,center,cite,code,dd,del,dfn,div,dl,dt,em,fieldset,font,form,h1,h2,h3,h4,h5,h6,html,i,iframe,img,ins,kbd,label,legend,li,object,p,pre,q,s,samp,small,span,strike,strong,sub,sup,table,tbody,td,tfoot,th,thead,tr,tt,u,ul,var{padding:0;margin:0;border:0;outline:none;vertical-align:baseline;background:0 0;text-decoration:none}dl,ul{list-style-position:inside;list-style:none}ul li{list-style:none}caption{text-align:center}img{border:none;position:relative}a,a:visited{text-decoration:none}.clearfix{clear:both}.section,.widget,.widget ul{margin:0;padding:0}a{color:var(--main-color)}a img{border:0}abbr{text-decoration:none}.CSS_LIGHTBOX{z-index:999999!important}.CSS_LIGHTBOX_ATTRIBUTION_INDEX_CONTAINER .CSS_HCONT_CHILDREN_HOLDER > .CSS_LAYOUT_COMPONENT.CSS_HCONT_CHILD:first-child > .CSS_LAYOUT_COMPONENT{opacity:0}.separator a{text-decoration:none!important;clear:none!important;float:none!important;margin-left:0!important;margin-right:0!important}#Navbar1,#navbar-iframe,.widget-item-control,a.quickedit,.home-link,.feed-links{display:none!important}.center{display:table;margin:0 auto;position:relative}.widget > h2,.widget > h3{display:none}.widget iframe,.widget img{max-width:100%}button,input,select,textarea{font-family:var(--body-font);-webkit-appearance:none;-moz-appearance:none;appearance:none;outline:none;border-radius:0}input[type="search"]::-webkit-search-cancel-button{-webkit-appearance:none}
/*-- Style CSS --*/
*{box-sizing:border-box}
html{position:relative;word-break:break-word;word-wrap:break-word;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-webkit-text-size-adjust:100%}
body{position:relative;background:var(--body-bg);background-color:var(--body-bg-color);font-family:var(--body-font);font-size:14px;color:var(--text-color);font-weight:400;font-style:normal;line-height:1.4em}
.rtl{direction:rtl}
h1,h2,h3,h4,h5,h6{font-family:var(--title-font);font-weight:700}
a,input,button{transition:all .0s ease}
#outer-wrapper{position:relative;overflow:hidden;width:100%;max-width:100%;background-color:var(--outer-bg);margin:0 auto;padding:0}
.is-boxed #outer-wrapper{width:$(row.width + 60px);max-width:100%;box-shadow:0 0 20px rgba(0,0,0,0.1)}
.is-dark .is-boxed #outer-wrapper{box-shadow:0 0 20px rgba(0,0,0,0.3)}
.container{position:relative}
.row-x1{width:$(row.width);max-width:100%}
.row-x2{width:100%}
.flex-center{display:flex;justify-content:center}
#content-wrapper{position:relative;float:left;width:100%;overflow:hidden;padding:20px 0;margin:0}
#content-wrapper > .container{display:flex;justify-content:space-between}
.is-left #content-wrapper > .container,.rtl .is-right #content-wrapper > .container{flex-direction:row-reverse}
.rtl .is-left #content-wrapper > .container{flex-direction:row}
.theiaStickySidebar:before,.theiaStickySidebar:after{content:'';display:table;clear:both}
#main-wrapper{position:relative;width:calc(100% - $(sidebar.width + 15px))}
.no-sidebar #main-wrapper{width:100%}
#sidebar-wrapper{position:relative;width:$(sidebar.width)}
.no-sidebar #sidebar-wrapper{display:none}
.btn{position:relative;border:0;border-radius:var(--radius)}
.entry-image-wrap,.author-avatar-wrap,.comments .avatar-image-container{display:block;position:relative;overflow:hidden;background-color:var(--rgba-gray);z-index:5;color:transparent!important}
.entry-thumb,.author-avatar{display:block;position:relative;width:100%;height:100%;background-size:cover;background-position:center center;background-repeat:no-repeat;z-index:1;opacity:0;transition:opacity .35s ease,filter 0s ease}
.author-avatar{background-size:100%;background-position:0 0}
.entry-thumb.lazy-ify,.author-avatar.lazy-ify{opacity:1}
.entry-image-wrap:hover .entry-thumb,.cs:hover .entry-image-wrap .entry-thumb{filter:brightness(1.03)}
.entry-image-wrap.is-video:after{position:absolute;content:'\f04b';top:50%;right:50%;width:38px;height:27px;background-color:rgba(0,0,0,0.5);font-family:'Font Awesome 5 Free';font-size:12px;color:#fff;font-weight:900;display:flex;align-items:center;justify-content:center;z-index:5;transform:translate(50%,-50%);box-sizing:border-box;padding:0 0 0 1px;margin:0;border-radius:var(--radius);box-shadow:0 1px 3px 0 rgb(0,0,0,0.1);transition:background .17s ease}
.entry-image-wrap.is-video:hover:after,.cs:hover .entry-image-wrap.is-video:after{background-color:#f50000}
.cs .entry-image-wrap.is-video:after{top:15px;right:15px;transform:translate(0)}
.rtl .cs .entry-image-wrap.is-video:after{left:15px;right:unset}
.entry-category{display:flex;width:-moz-fit-content;width:fit-content;height:20px;background-color:var(--main-color);font-size:12px;color:#fff;align-items:center;padding:0 10px;margin:0 0 10px;border-radius:20px}
.entry-title{display:block;color:var(--post-title-color);font-weight:500;line-height:1.4em}
.entry-title a{display:block;color:var(--post-title-color)}
.entry-title a:hover{color:var(--post-title-hover-color)}
.entry-meta{display:flex;font-size:12px;color:var(--meta-color);font-weight:400;margin:4px 0 0}
.entry-meta .mi{display:flex}
.entry-meta .mi,.entry-meta .sp{margin:0 3px 0 0}
.rtl .entry-meta .mi,.rtl .entry-meta .sp{margin:0 0 0 3px}
.entry-meta .author-name{color:var(--main-color);font-weight:500}
.excerpt{font-family:var(--text-font);line-height:1.5em}
.before-mask:before{content:'';position:absolute;left:0;right:0;bottom:0;height:100%;background-image:linear-gradient(to bottom,rgba(0,0,0,0) 30%,rgba(0,0,0,0.5));-webkit-backface-visibility:hidden;backface-visibility:hidden;z-index:2;opacity:1;margin:0;transition:opacity .25s ease}
.cs{overflow:hidden}
.entry-info{position:absolute;left:0;bottom:0;width:100%;background:linear-gradient(to bottom,rgba(0,0,0,0),rgba(0,0,0,0.5));overflow:hidden;z-index:10;display:flex;flex-direction:column;padding:16px}
.entry-info .entry-title{color:#fff;text-shadow:0 1px 2px rgba(0,0,0,0.1)}
.entry-info .entry-meta{color:#c5c5c5;text-shadow:0 1px 2px rgba(0,0,0,0.1)}
.entry-info .entry-meta .author-name{color:#d5d5d5;font-weight:400}
.error-msg{display:flex;align-items:center;font-size:14px;color:var(--meta-color);padding:20px 0;font-weight:400}
.error-msg b{font-weight:500}
.loader{position:relative;width:100%;height:100%;overflow:hidden;display:flex;align-items:center;justify-content:center;margin:0}
.loader:after{content:'';display:block;width:30px;height:30px;box-sizing:border-box;margin:0;border:1.45px solid var(--main-color);border-right-color:var(--border-color);border-radius:100%;animation:spinner .65s infinite linear;transform-origin:center}
@-webkit-keyframes spinner {
0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}
to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}
}
@keyframes spinner {
0%{-webkit-transform:rotate(0deg);transform:rotate(0deg)}
to{-webkit-transform:rotate(1turn);transform:rotate(1turn)}
}
.social a:before{display:inline-block;font-family:'Font Awesome 5 Brands';font-style:normal;font-weight:400}
.social .blogger a:before{content:'\f37d'}
.social .apple a:before{content:'\f179'}
.social .amazon a:before{content:'\f270'}
.social .microsoft a:before{content:'\f3ca'}
.social .facebook a:before{content:'\f09a'}
.social .facebook-f a:before{content:'\f39e'}
.social .twitter a:before{content:'\f099'}
.social .rss a:before{content:'\f09e';font-family:'Font Awesome 5 Free';font-weight:900}
.social .youtube a:before{content:'\f167'}
.social .skype a:before{content:'\f17e'}
.social .stumbleupon a:before{content:'\f1a4'}
.social .tumblr a:before{content:'\f173'}
.social .vk a:before{content:'\f189'}
.social .stack-overflow a:before{content:'\f16c'}
.social .github a:before{content:'\f09b'}
.social .linkedin a:before{content:'\f0e1'}
.social .dribbble a:before{content:'\f17d'}
.social .soundcloud a:before{content:'\f1be'}
.social .behance a:before{content:'\f1b4'}
.social .digg a:before{content:'\f1a6'}
.social .instagram a:before{content:'\f16d'}
.social .pinterest a:before{content:'\f0d2'}
.social .pinterest-p a:before{content:'\f231'}
.social .twitch a:before{content:'\f1e8'}
.social .delicious a:before{content:'\f1a5'}
.social .codepen a:before{content:'\f1cb'}
.social .flipboard a:before{content:'\f44d'}
.social .reddit a:before{content:'\f281'}
.social .whatsapp a:before{content:'\f232'}
.social .messenger a:before{content:'\f39f'}
.social .snapchat a:before{content:'\f2ac'}
.social .telegram a:before{content:'\f3fe'}
.social .steam a:before{content:'\f3f6'}
.social .discord a:before{content:'\f392'}
.social .quora a:before{content:'\f2c4'}
.social .tiktok a:before{content:'\e07b'}
.social .share a:before{content:'\f064';font-family:'Font Awesome 5 Free';font-weight:900}
.social .email a:before{content:'\f0e0';font-family:'Font Awesome 5 Free'}
.social .external-link a:before{content:'\f35d';font-family:'Font Awesome 5 Free';font-weight:900}
.social-bg .blogger a,.social-bg-hover .blogger a:hover{background-color:#ff5722}
.social-bg .apple a,.social-bg-hover .apple a:hover{background-color:#333}
.social-bg .amazon a,.social-bg-hover .amazon a:hover{background-color:#fe9800}
.social-bg .microsoft a,.social-bg-hover .microsoft a:hover{background-color:#0067B8}
.social-bg .facebook a,.social-bg .facebook-f a,.social-bg-hover .facebook a:hover,.social-bg-hover .facebook-f a:hover{background-color:#3b5999}
.social-bg .twitter a,.social-bg-hover .twitter a:hover{background-color:#00acee}
.social-bg .youtube a,.social-bg-hover .youtube a:hover{background-color:#f50000}
.social-bg .instagram a,.social-bg-hover .instagram a:hover{background:linear-gradient(15deg,#ffb13d,#dd277b,#4d5ed4)}
.social-bg .pinterest a,.social-bg .pinterest-p a,.social-bg-hover .pinterest a:hover,.social-bg-hover .pinterest-p a:hover{background-color:#ca2127}
.social-bg .dribbble a,.social-bg-hover .dribbble a:hover{background-color:#ea4c89}
.social-bg .linkedin a,.social-bg-hover .linkedin a:hover{background-color:#0077b5}
.social-bg .tumblr a,.social-bg-hover .tumblr a:hover{background-color:#365069}
.social-bg .twitch a,.social-bg-hover .twitch a:hover{background-color:#6441a5}
.social-bg .rss a,.social-bg-hover .rss a:hover{background-color:#ffc200}
.social-bg .skype a,.social-bg-hover .skype a:hover{background-color:#00aff0}
.social-bg .stumbleupon a,.social-bg-hover .stumbleupon a:hover{background-color:#eb4823}
.social-bg .vk a,.social-bg-hover .vk a:hover{background-color:#4a76a8}
.social-bg .stack-overflow a,.social-bg-hover .stack-overflow a:hover{background-color:#f48024}
.social-bg .github a,.social-bg-hover .github a:hover{background-color:#24292e}
.social-bg .soundcloud a,.social-bg-hover .soundcloud a:hover{background:linear-gradient(#ff7400,#ff3400)}
.social-bg .behance a,.social-bg-hover .behance a:hover{background-color:#191919}
.social-bg .digg a,.social-bg-hover .digg a:hover{background-color:#1b1a19}
.social-bg .delicious a,.social-bg-hover .delicious a:hover{background-color:#0076e8}
.social-bg .codepen a,.social-bg-hover .codepen a:hover{background-color:#000}
.social-bg .flipboard a,.social-bg-hover .flipboard a:hover{background-color:#f52828}
.social-bg .reddit a,.social-bg-hover .reddit a:hover{background-color:#ff4500}
.social-bg .whatsapp a,.social-bg-hover .whatsapp a:hover{background-color:#3fbb50}
.social-bg .messenger a,.social-bg-hover .messenger a:hover{background-color:#0084ff}
.social-bg .snapchat a,.social-bg-hover .snapchat a:hover{background-color:#ffe700}
.social-bg .telegram a,.social-bg-hover .telegram a:hover{background-color:#179cde}
.social-bg .steam a,.social-bg-hover .steam a:hover{background:linear-gradient(5deg,#0d89bc,#112c5b,#0d1c47)}
.social-bg .discord a,.social-bg-hover .discord a:hover{background-color:#7289da}
.social-bg .quora a,.social-bg-hover .quora a:hover{background-color:#b92b27}
.social-bg .tiktok a,.social-bg-hover .tiktok a:hover{background-color:#fe2c55}
.social-bg .share a,.social-bg-hover .share a:hover{background-color:var(--meta-color)}
.social-bg .email a,.social-bg-hover .email a:hover{background-color:#888}
.social-bg .external-link a,.social-bg-hover .external-link a:hover{background-color:var(--title-color)}
.social-color .blogger a,.social-color-hover .blogger a:hover{color:#ff5722}
.social-color .apple a,.social-color-hover .apple a:hover{color:#333}
.social-color .amazon a,.social-color-hover .amazon a:hover{color:#fe9800}
.social-color .microsoft a,.social-color-hover .microsoft a:hover{color:#0067B8}
.social-color .facebook a,.social-color .facebook-f a,.social-color-hover .facebook a:hover,.social-color-hover .facebook-f a:hover{color:#3b5999}
.social-color .twitter a,.social-color-hover .twitter a:hover{color:#00acee}
.social-color .youtube a,.social-color-hover .youtube a:hover{color:#f50000}
.social-color .instagram a,.social-color-hover .instagram a:hover{color:#dd277b}
.social-color .pinterest a,.social-color .pinterest-p a,.social-color-hover .pinterest a:hover,.social-color-hover .pinterest-p a:hover{color:#ca2127}
.social-color .dribbble a,.social-color-hover .dribbble a:hover{color:#ea4c89}
.social-color .linkedin a,.social-color-hover .linkedin a:hover{color:#0077b5}
.social-color .tumblr a,.social-color-hover .tumblr a:hover{color:#365069}
.social-color .twitch a,.social-color-hover .twitch a:hover{color:#6441a5}
.social-color .rss a,.social-color-hover .rss a:hover{color:#ffc200}
.social-color .skype a,.social-color-hover .skype a:hover{color:#00aff0}
.social-color .stumbleupon a,.social-color-hover .stumbleupon a:hover{color:#eb4823}
.social-color .vk a,.social-color-hover .vk a:hover{color:#4a76a8}
.social-color .stack-overflow a,.social-color-hover .stack-overflow a:hover{color:#f48024}
.social-color .github a,.social-color-hover .github a:hover{color:#24292e}
.social-color .soundcloud a,.social-color-hover .soundcloud a:hover{color:#ff7400}
.social-color .behance a,.social-color-hover .behance a:hover{color:#191919}
.social-color .digg a,.social-color-hover .digg a:hover{color:#1b1a19}
.social-color .delicious a,.social-color-hover .delicious a:hover{color:#0076e8}
.social-color .codepen a,.social-color-hover .codepen a:hover{color:#000}
.social-color .flipboard a,.social-color-hover .flipboard a:hover{color:#f52828}
.social-color .reddit a,.social-color-hover .reddit a:hover{color:#ff4500}
.social-color .whatsapp a,.social-color-hover .whatsapp a:hover{color:#3fbb50}
.social-color .messenger a,.social-color-hover .messenger a:hover{color:#0084ff}
.social-color .snapchat a,.social-color-hover .snapchat a:hover{color:#ffe700}
.social-color .telegram a,.social-color-hover .telegram a:hover{color:#179cde}
.social-color .steam a,.social-color-hover .steam a:hover{color:#112c5b}
.social-color .discord a,.social-color-hover .discord a:hover{color:#7289da}
.social-color .quora a,.social-color-hover .quora a:hover{color:#b92b27}
.social-color .tiktok a,.social-color-hover .tiktok a:hover{color:#fe2c55}
.social-color .share a,.social-color-hover .share a:hover{color:var(--meta-color)}
.social-color .email a,.social-color-hover .email a:hover{color:#888}
.social-color .external-link a,.social-color-hover .external-link a:hover{color:var(--title-color)}
#header-wrapper{position:relative;float:left;width:100%;z-index:50;margin:0}
.main-header,.header-inner{position:relative;float:left;width:100%;height:59px;background-color:var(--header-bg)}
.header-inner{background-color:rgba(0,0,0,0)}
.header-inner.is-fixed{position:fixed;top:-59px;left:0;width:100%;z-index:990;backface-visibility:hidden;visibility:hidden;opacity:0;transition:all .25s ease}
.header-inner.is-fixed.show{top:0;opacity:1;visibility:visible;margin:0}
.header-header{position:relative;float:left;width:100%;height:59px;background-color:var(--header-bg);border-bottom:1px solid var(--border-color)}
.is-boxed .header-header{float:none;width:$(row.width + 60px);max-width:100%;margin:0 auto;padding:0}
.is-fixed .header-header{box-shadow:0 1px 8px rgba(0,0,0,0.1)}
.header-items{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between}
.flex-left{position:static;display:flex;z-index:10}
.flex-right{position:absolute;top:0;right:0;z-index:20}
.rtl .flex-right{left:0;right:unset}
.main-logo{position:relative;float:left;height:58px;overflow:hidden;padding:0 13px 0 0}
.rtl .main-logo{padding:0 0 0 13px}
.main-logo .widget{position:relative;height:100%;display:flex;align-items:center}
.main-logo .logo-img{display:flex;align-items:center;height:34px;overflow:hidden}
.main-logo img{display:block;max-width:100%;max-height:100%}
.main-logo .blog-title{display:block;font-size:23px;color:var(--header-color);font-weight:700}
.main-logo .blog-title a{color:var(--header-color)}
.main-logo .blog-title a:hover{color:var(--header-hover-color)}
.main-logo #h1-off{position:absolute;top:-9000px;left:-9000px;display:none;visibility:hidden}
#litespot-pro-main-nav{position:static;height:58px;z-index:10}
#litespot-pro-main-nav .widget,#litespot-pro-main-nav .widget > .widget-title{display:none}
#litespot-pro-main-nav .show-menu{display:block}
#litespot-pro-main-nav ul#litespot-pro-main-nav-menu{display:flex;flex-wrap:wrap}
#litespot-pro-main-nav ul > li{position:relative;padding:0;margin:0}
#litespot-pro-main-nav-menu > li > a{position:relative;display:block;height:58px;font-family:var(--menu-font);font-size:15px;color:var(--header-color);font-weight:600;line-height:58px;padding:0 14px;margin:0}
#litespot-pro-main-nav-menu > li:hover > a{color:var(--header-hover-color)}
#litespot-pro-main-nav ul > li > ul,#litespot-pro-main-nav ul > li > .ul{position:absolute;left:0;top:58px;width:180px;background-color:var(--submenu-bg);z-index:99999;padding:5px 0;backface-visibility:hidden;visibility:hidden;opacity:0;transform:translate3d(0,-10px,0);border-radius:var(--radius);box-shadow:0 1px 2px rgba(0,0,0,0.1),0 5px 10px 0 rgba(0,0,0,0.1)}
.rtl #litespot-pro-main-nav ul > li > ul,.rtl #litespot-pro-main-nav ul > li > .ul{left:auto;right:0}
#litespot-pro-main-nav ul > li > ul > li > ul{position:absolute;top:-5px;left:100%;transform:translate3d(-10px,0,0);margin:0}
.rtl #litespot-pro-main-nav ul > li > ul > li > ul{left:unset;right:100%;transform:translate3d(10px,0,0)}
#litespot-pro-main-nav ul > li > ul > li{display:block;float:none;position:relative}
.rtl #litespot-pro-main-nav ul > li > ul > li{float:none}
#litespot-pro-main-nav ul > li > ul > li a{position:relative;display:block;font-size:14px;color:var(--submenu-color);font-weight:400;padding:8px 14px;margin:0}
#litespot-pro-main-nav ul > li > ul > li:hover > a{color:var(--submenu-hover-color)}
#litespot-pro-main-nav ul > li.has-sub > a:after{content:'\f078';float:right;font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:3px 0 0 4px}
.rtl #litespot-pro-main-nav ul > li.has-sub > a:after{float:left;margin:3px 4px 0 0}
#litespot-pro-main-nav ul > li > ul > li.has-sub > a:after{content:'\f054';float:right;margin:0}
.rtl #litespot-pro-main-nav ul > li > ul > li.has-sub > a:after{content:'\f053'}
#litespot-pro-main-nav ul ul,#litespot-pro-main-nav ul .ul{transition:visibility .1s ease,opacity .17s ease,transform .17s ease}
#litespot-pro-main-nav ul > li:hover > ul,#litespot-pro-main-nav ul > li:hover > .ul,#litespot-pro-main-nav ul > li > ul > li:hover > ul{visibility:visible;opacity:1;transform:translate3d(0,0,0);margin:0}
#litespot-pro-main-nav .mega-menu{position:static!important}
#litespot-pro-main-nav .mega-menu > .ul{width:100%;background-color:var(--megamenu-bg);overflow:hidden;padding:20px}
.mega-menu .mega-items{display:grid;grid-template-columns:repeat(5,1fr);column-gap:20px}
.mega-menu .mega-items.no-items{grid-template-columns:1fr}
.mega-items .mega-item{position:relative;width:100%;display:flex;flex-direction:column;padding:0}
.mega-item .entry-image-wrap{width:100%;height:124px;z-index:1;margin:0 0 8px;border-radius:var(--radius)}
.mega-item .entry-title{font-size:14px}
.mega-item .entry-title a{color:var(--megamenu-color)}
.mega-item .entry-title a:hover{color:var(--megamenu-hover-color)}
.mega-menu .error-msg{justify-content:center}
.mobile-menu-toggle{display:none;height:34px;font-size:18px;color:var(--header-color);align-items:center;padding:0 16px}
.mobile-menu-toggle:after{content:'\f0c9';font-family:'Font Awesome 5 Free';font-weight:900;margin:0}
.mobile-menu-toggle:hover{color:var(--header-hover-color)}
.tgl-wrap{height:58px;background-color:var(--header-bg);display:flex;align-items:center;z-index:20;margin:0}
.tgl-style{width:38px;height:38px;background-color:var(--rgba-gray);color:var(--header-color);font-size:16px;display:flex;align-items:center;justify-content:center;cursor:pointer;z-index:20;border-radius:var(--radius)}
.darkmode-toggle{width:auto;background-color:transparent;font-size:14px;padding:0 15px}
.tgl-style:after{content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900}
.darkmode-toggle:after{content:'\f186';font-weight:400}
.is-dark .darkmode-toggle:after{content:'\f185';font-weight:900}
.show-search{transition:opacity .17s ease}
.tgl-style:hover{color:var(--header-hover-color)}
#main-search-wrap{display:none;position:absolute;top:0;right:0;width:$(sidebar.width);height:58px;background-color:var(--header-bg);z-index:25}
.rtl #main-search-wrap{left:0;right:unset}
@-webkit-keyframes showSearch {
0%{width:80%;opacity:0}
100%{width:100%;opacity:1}
}
.main-search{position:relative;float:right;width:100%;height:100%;display:flex;align-items:center;animation:showSearch .17s ease}
.rtl .main-search{float:left}
.main-search .search-form{position:relative;height:38px;background-color:var(--rgba-gray);display:flex;flex:1;border:0;border-radius:var(--radius)}
.main-search .search-form:focus-within{background-color:var(--header-bg);box-shadow:0 1px 1px rgba(0,0,0,0.1),0 1px 3px rgba(0,0,0,0.2)}
.is-dark .main-search .search-form:focus-within{background-color:var(--rgba-gray)}
.main-search .search-input{width:100%;flex:1;background-color:rgba(0,0,0,0);font-family:inherit;font-size:14px;color:var(--header-color);font-weight:400;text-align:left;padding:0 16px;border:0}
.rtl .main-search .search-input{text-align:right}
.main-search .search-input:focus,.main-search .search-input::placeholder{color:var(--header-color);outline:none}
.main-search .search-input::placeholder{opacity:.65}
.main-search .search-close{width:38px;background-color:rgba(0,0,0,0);font-size:16px;color:var(--header-color);text-align:center;cursor:pointer;border:0}
.main-search .search-close:before{display:block;content:'\f00d';font-family:'Font Awesome 5 Free';font-weight:900}
.main-search .search-close:hover{color:var(--header-hover-color)}
.overlay{visibility:hidden;opacity:0;position:fixed;top:0;left:0;right:0;bottom:0;background-color:rgba(27,27,37,0.6);z-index:1000;-webkit-backdrop-filter:saturate(100%) blur(3px);-ms-backdrop-filter:saturate(100%) blur(3px);-o-backdrop-filter:saturate(100%) blur(3px);backdrop-filter:saturate(100%) blur(3px);margin:0;transition:all .25s ease}
#slide-menu{display:none;position:fixed;width:300px;height:100%;top:0;left:0;bottom:0;background-color:var(--mobilemenu-bg);overflow:hidden;z-index:1010;left:0;-webkit-transform:translateX(-100%);transform:translateX(-100%);visibility:hidden;box-shadow:3px 0 7px rgba(0,0,0,0.1);transition:all .25s ease}
.rtl #slide-menu{left:unset;right:0;-webkit-transform:translateX(100%);transform:translateX(100%)}
.nav-active #slide-menu,.rtl .nav-active #slide-menu{-webkit-transform:translateX(0);transform:translateX(0);visibility:visible}
.slide-menu-header{position:relative;float:left;width:100%;height:59px;background-color:var(--mobilemenu-bg);overflow:hidden;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid var(--border-color)}
.mobile-search{flex:1;padding:0 0 0 16px}
.rtl .mobile-search{padding:0 16px 0 0}
.mobile-search .search-form{width:100%;height:34px;background-color:var(--rgba-gray);overflow:hidden;display:flex;justify-content:space-between;border:0;border-radius:var(--radius)}
.mobile-search .search-form:focus-within{background-color:var(--mobilemenu-bg);box-shadow:0 1px 1px rgba(0,0,0,0.1),0 1px 3px rgba(0,0,0,0.2)}
.is-dark .mobile-search .search-form:focus-within{background-color:var(--rgba-gray)}
.mobile-search .search-input{flex:1;width:100%;background-color:rgba(0,0,0,0);font-family:inherit;font-size:14px;color:var(--mobilemenu-color);font-weight:400;padding:0 10px;border:0}
.mobile-search .search-input:focus,.mobile-search .search-input::placeholder{color:var(--mobilemenu-color)}
.mobile-search .search-input::placeholder{opacity:.65}
.mobile-search .search-action{background-color:rgba(0,0,0,0);font-family:inherit;font-size:12px;color:var(--mobilemenu-color);font-weight:400;text-align:center;cursor:pointer;padding:0 10px;border:0;opacity:.65}
.mobile-search .search-action:before{display:block;content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900}
.mobile-search .search-action:hover{opacity:1}
.hide-litespot-pro-mobile-menu{display:flex;height:100%;color:var(--mobilemenu-color);font-size:16px;align-items:center;cursor:pointer;z-index:20;padding:0 16px}
.hide-litespot-pro-mobile-menu:before{content:'\f00d';font-family:'Font Awesome 5 Free';font-weight:900}
.hide-litespot-pro-mobile-menu:hover{color:var(--mobilemenu-hover-color)}
.slide-menu-flex{position:relative;float:left;width:100%;height:calc(100% - 59px);display:flex;flex-direction:column;justify-content:space-between;overflow:hidden;overflow-y:auto;-webkit-overflow-scrolling:touch;margin:0}
.litespot-pro-mobile-menu{position:relative;float:left;width:100%;padding:16px}
.litespot-pro-mobile-menu .m-sub{display:none}
.litespot-pro-mobile-menu ul li{position:relative;display:block;overflow:hidden;float:left;width:100%;margin:0}
.litespot-pro-mobile-menu > ul li ul{overflow:hidden}
.litespot-pro-mobile-menu ul li a{font-size:15px;color:var(--mobilemenu-color);font-weight:400;padding:8px 0;display:block}
.litespot-pro-mobile-menu > ul > li > a{font-family:var(--menu-font);font-weight:600}
.litespot-pro-mobile-menu ul li.has-sub .submenu-toggle{position:absolute;top:0;right:0;width:30px;color:var(--mobilemenu-color);text-align:right;cursor:pointer;padding:8px 0}
.rtl .litespot-pro-mobile-menu ul li.has-sub .submenu-toggle{text-align:left;right:auto;left:0}
.litespot-pro-mobile-menu ul li.has-sub .submenu-toggle:after{content:'\f078';font-family:'Font Awesome 5 Free';font-weight:900;float:right;font-size:12px;text-align:right;transition:all 0s ease}
.rtl .litespot-pro-mobile-menu ul li.has-sub .submenu-toggle:after{float:left}
.litespot-pro-mobile-menu ul li.has-sub.show > .submenu-toggle:after{content:'\f077'}
.litespot-pro-mobile-menu ul li a:hover,.litespot-pro-mobile-menu ul li.has-sub.show > a,.litespot-pro-mobile-menu ul li.has-sub.show > .submenu-toggle{color:var(--mobilemenu-hover-color)}
.litespot-pro-mobile-menu > ul > li > ul > li a{font-size:14px;opacity:.75;padding:8px 0 8px 10px}
.rtl .litespot-pro-mobile-menu > ul > li > ul > li a{padding:8px 10px 8px 0}
.litespot-pro-mobile-menu > ul > li > ul > li > ul > li > a{padding:8px 0 8px 20px}
.rtl .litespot-pro-mobile-menu > ul > li > ul > li > ul > li > a{padding:8px 20px 8px 0}
.litespot-pro-mobile-menu ul > li > .submenu-toggle:hover{color:var(--mobilemenu-hover-color)}
.mm-footer{position:relative;float:left;width:100%;padding:20px 16px;margin:0}
.mm-footer .mm-social,.mm-footer .mm-menu{position:relative;float:left;width:100%;margin:8px 0 0}
.mm-footer .mm-social{margin:0}
.mm-footer ul{display:flex;flex-wrap:wrap}
.mm-footer .mm-social ul li{margin:0 16px 0 0}
.rtl .mm-footer .mm-social ul li{margin:0 0 0 16px}
.mm-footer .mm-social ul li:last-child{margin:0}
.mm-footer .mm-social ul li a{display:block;font-size:14px;color:var(--mobilemenu-color);padding:0}
.mm-footer .mm-social ul li a:hover{color:var(--mobilemenu-hover-color)}
.mm-footer .mm-menu ul li{margin:5px 18px 0 0}
.rtl .mm-footer .mm-menu ul li{margin:5px 0 0 18px}
.mm-footer .mm-menu ul li:last-child{margin:5px 0 0}
.mm-footer .mm-menu ul li a{display:block;font-size:14px;color:var(--mobilemenu-color);font-weight:400;padding:0}
.mm-footer .mm-menu ul li a:hover{color:var(--mobilemenu-hover-color)}
#header-ads-wrap{position:relative;float:left;width:100%;margin:0}
.header-ads .widget,.header-ads .widget-content{position:relative;float:left;width:100%;margin:0}
.header-ads .widget{margin:20px 0 0}
#ticker-wrapper,#ticker .widget{position:relative;float:left;width:100%;margin:0}
#ticker .widget{display:none;background-color:var(--widget-bg);align-items:flex-start;padding:16px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
#ticker .widget.is-visible,#ticker .widget.PopularPosts{display:flex}
.ticker .widget-title{padding:0 8px 0 0}
.rtl .ticker .widget-title{padding:0 0 0 8px}
.ticker .widget-title .title{font-size:15px;color:var(--main-color);font-weight:700;line-height:20px}
.ticker .widget-content{position:relative;height:20px;display:flex;justify-content:space-between;flex:1;margin:0}
.ticker .loader{justify-content:flex-start}
.ticker .loader:after{width:20px;height:20px}
.ticker .error-msg{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis;padding:0}
.ticker-items{position:relative;display:flex;align-items:center;flex:1;overflow:hidden}
.ticker-item{position:absolute;top:0;left:0;width:100%;opacity:0;visibility:hidden;transform:translate3d(10px,0,0);pointer-events:none;transition:all .85s ease}
.rtl .ticker-item{left:unset;right:0;transform:translate3d(-10px,0,0)}
.ticker-item.active{opacity:1;visibility:visible;transform:translate3d(0,0,0);pointer-events:initial}
.ticker-item .entry-title{height:20px;display:flex;font-size:15px;font-weight:600;line-height:20px}
.ticker-item .entry-title a{max-width:100%;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}
.ticker-nav{display:grid;grid-template-columns:1fr 1fr;grid-gap:5px;padding:0 0 0 10px}
.rtl .ticker-nav{padding:0 10px 0 0}
.ticker-nav a{display:flex;width:20px;height:20px;background-color:var(--rgba-gray);font-size:9px;color:var(--title-color);align-items:center;justify-content:center;border-radius:var(--radius)}
.ticker-nav a:hover{color:var(--main-color)}
.ticker-nav a:before{display:block;font-family:'Font Awesome 5 Free';font-weight:900}
.ticker-nav .tn-prev:before,.rtl .ticker-nav a.tn-next:before{content:'\f053'}
.ticker-nav a.tn-next:before,.rtl .ticker-nav .tn-prev:before{content:'\f054'}
#featured-wrapper,#featured .widget,#featured .widget-content{position:relative;float:left;width:100%;margin:0}
#featured .widget{display:none;margin:20px 0 0}
#featured .widget.is-visible,#featured .widget.PopularPosts{display:block}
#featured .widget-content{display:flex;align-items:center;justify-content:center;min-height:200px;margin:0}
#featured .error-msg{padding:0}
.featured-items{position:relative;float:left;width:100%;display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px}
.featured-item{position:relative;width:100%;height:200px}
.featured-inner{position:relative;width:100%;height:100%;display:flex;flex-direction:column;z-index:11;overflow:hidden;border-radius:var(--radius)}
.featured-item .entry-image-wrap{width:100%;height:100%}
.featured-item .entry-title{font-size:17px}
.featured-item .entry-meta{flex-wrap:wrap}
.title-wrap{position:relative;float:left;width:100%;display:flex;align-items:center;justify-content:space-between;margin:0 0 16px}
.title-wrap > *{display:flex;align-items:center}
.title-wrap > .title{font-family:var(--title-font);font-size:16px;color:var(--widget-title-color);font-weight:700;margin:0}
.title-wrap > .title:after{content:'\f054';font-family:'Font Awesome 5 Free';font-size:10px;font-weight:900;line-height:1;margin:2px 0 0 3px}
.rtl .title-wrap > .title:after{content:'\f053';margin:2px 3px 0 0}
.title-wrap > a.wt-l{font-size:12px;color:var(--meta-color);font-weight:400;line-height:1}
.title-wrap > a.wt-l:hover{color:var(--main-color)}
.content-section,.content-section .widget,.content-section .widget-content,.content-section .content-block{position:relative;float:left;width:100%;margin:0}
.content-section .widget{display:none;margin:0 0 20px}
.content-section .widget.is-visible,.content-section .widget.is-ad{display:block}
#content-section-2 .widget:last-child{margin:0}
.content-section .loader{height:200px}
.block-items{display:grid;grid-template-columns:repeat(2,1fr);grid-gap:20px}
.block-left,.block-right{position:relative;width:100%;margin:0}
.block-right{display:flex;flex-direction:column}
.block-item{position:relative;width:100%;background-color:var(--post-card-bg);display:flex;flex-direction:column;border:1px solid var(--border-color);border-radius:var(--radius)}
.block-left .block-item{overflow:hidden}
.block-left .entry-image-wrap{width:100%;height:205px;border-radius:var(--radius) var(--radius) 0 0}
.block-left .entry-header{padding:13px 16px 16px}
.block-left .entry-title{font-size:20px}
.block-left .entry-meta{flex-wrap:wrap;margin:6px 0 0}
.block-right .block-item{flex-direction:row;padding:10px;margin:20px 0 0}
.block-right .block-item.item-1{margin:0}
.block-right .entry-header{display:flex;flex-direction:column;flex:1}
.block-right .entry-image-wrap{width:100px;height:65px;margin:0 12px 0 0;border-radius:var(--radius)}
.rtl .block-right .entry-image-wrap{margin:0 0 0 12px}
.block-right .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.75)}
.block-right .entry-title{font-size:15px}
.grid-items{display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px}
.grid-item{position:relative;background-color:var(--post-card-bg);display:flex;flex-direction:column;overflow:hidden;border:1px solid var(--border-color);border-radius:var(--radius)}
.grid-item .entry-image-wrap{width:100%;height:140px;border-radius:var(--radius) var(--radius) 0 0}
.grid-item .entry-header{padding:13px 10px}
.grid-item .entry-title{font-size:15px}
.list-items{display:flex;flex-direction:column}
.list-item{position:relative;width:100%;background-color:var(--post-card-bg);display:flex;padding:16px 12px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.list-item.item-0{margin:0}
.list-item .entry-image-wrap{width:200px;height:133px;margin:0 16px 0 0;border-radius:var(--radius)}
.rtl .list-item .entry-image-wrap{margin:0 0 0 16px}
.list-item .entry-header{display:flex;flex-direction:column;flex:1;margin:0}
.list-item .entry-title{font-size:20px;margin:0}
.list-item .entry-excerpt{font-size:14px;color:var(--text-color);margin:8px 0 0}
.list-item .entry-meta{flex-wrap:wrap;font-size:12px;margin:8px 0 0}
.video-items{display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px}
.video-item{position:relative;background-color:var(--post-card-bg);display:flex;flex-direction:column;overflow:hidden;border:1px solid var(--border-color);border-radius:var(--radius)}
.video-item .entry-image-wrap{width:100%;height:140px;border-radius:var(--radius) var(--radius) 0 0}
.video-item .entry-header{padding:13px 10px}
.video-item .entry-title{font-size:15px}
#main-wrapper #main,#main .Blog{position:relative;float:left;width:100%;margin:0}
.is-home #main-wrapper.has-cs2 #main{margin:0 0 20px}
.blog-posts-wrap{position:relative;float:left;width:100%}
.queryMessage{float:left;width:100%}
.queryMessage .query-info,.Blog.no-posts .queryMessage{margin:0}
.queryMessage .query-info{position:relative;float:left;width:100%;display:flex;align-items:center;font-family:var(--title-font);font-size:16px;color:var(--widget-title-color);font-weight:700;margin:0 0 16px}
.queryMessage .query-info:after{content:'\f054';font-family:'Font Awesome 5 Free';font-size:10px;font-weight:900;line-height:1;margin:1px 0 0 3px}
.rtl .queryMessage .query-info:after{content:'\f053';margin:1px 3px 0 0}
.queryEmpty{float:left;width:100%;font-size:14px;color:var(--text-color);font-weight:400;text-align:center;margin:50px 0}
.index-post-wrap{position:relative;float:left;width:100%;display:flex;flex-direction:column}
.no-posts .index-post-wrap{display:none}
.blog-post{display:block;word-wrap:break-word}
.index-post{position:relative;width:100%;background-color:var(--post-card-bg);display:flex;padding:16px 12px;margin:0 0 20px;border:1px solid var(--border-color);border-radius:var(--radius)}
.index-post.ad-type{display:block;background-color:transparent;padding:0;border:0;border-radius:0}
.index-post-wrap .index-post:last-child{margin:0}
.index-post .entry-image-wrap{width:200px;height:133px;margin:0 16px 0 0;border-radius:var(--radius)}
.rtl .index-post .entry-image-wrap{margin:0 0 0 16px}
.index-post .entry-header{display:flex;flex-direction:column;flex:1;margin:0}
.index-post .entry-title{font-size:20px}
.index-post .entry-excerpt{font-size:14px;color:var(--text-color);margin:8px 0 0}
.index-post .entry-meta{flex-wrap:wrap;font-size:12px;margin:8px 0 0}
.inline-ad-wrap{position:relative;float:left;width:100%;margin:0}
.inline-ad{position:relative;float:left;width:100%;text-align:center;line-height:1;margin:0}
.post-animated{-webkit-animation-duration:.5s;animation-duration:.5s}
@keyframes fadeInUp {
from{opacity:0;transform:translate3d(0,10px,0)}
to{opacity:1;transform:translate3d(0,0,0)}
}
.post-fadeInUp{animation-name:fadeInUp}
.item-post-wrap,.is-single .item-post,.item-post-inner{position:relative;float:left;width:100%;margin:0}
.item-post .blog-entry-header{position:relative;float:left;width:100%;display:flex;flex-direction:column}
#breadcrumb{float:left;display:flex;width:100%;font-size:14px;color:var(--meta-color);font-weight:400;line-height:1;margin:0 0 10px}
#breadcrumb a{color:var(--meta-color)}
#breadcrumb a.home,#breadcrumb a:hover{color:var(--main-color)}
#breadcrumb em:after{content:'\f054';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;font-style:normal;vertical-align:middle;margin:0 4px}
.rtl #breadcrumb em:after{content:'\f053'}
.item-post h1.entry-title{position:relative;float:left;width:100%;font-size:$(itempost.title.size);font-weight:400;margin:0}
.item-post .has-meta h1.entry-title{margin-bottom:12px}
.p-eh .entry-meta{flex-wrap:wrap;justify-content:space-between;font-size:14px;margin:0}
.p-eh .entry-meta .align-left,.p-eh .entry-meta .align-right{display:flex;flex-wrap:wrap;align-items:center}
.p-eh .entry-meta .mi,.p-eh .entry-meta .sp{margin:0 4px 0 0}
.rtl .p-eh .entry-meta .mi,.rtl .p-eh .entry-meta .sp{margin:0 0 0 4px}
.p-eh .entry-meta .entry-author{align-items:center}
.p-eh .entry-meta .entry-author:before{display:none}
.p-eh .entry-meta .author-avatar-wrap{overflow:visible;width:30px;height:30px;background-color:var(--widget-bg);padding:1px;margin:0 5px 0 0;border:1px solid var(--main-color);border-radius:100%}
.rtl .p-eh .entry-meta .author-avatar-wrap{margin:0 0 0 5px}
.p-eh .entry-meta .author-avatar-wrap:before{content:'';position:absolute;display:block;top:calc(50% - 6px);left:-1px;width:calc(100% + 2px);height:12px;background-color:var(--widget-bg);z-index:1;margin:0}
.p-eh .entry-meta .author-avatar{z-index:2;border-radius:50%}
.p-eh .entry-meta .author-name{font-weight:400}
.entry-meta .entry-comments-link{display:none;margin:0 0 0 10px}
.rlt .entry-meta .entry-comments-link{margin:0 10px 0 0}
.entry-meta .entry-comments-link:before{display:inline-block;content:'\f086';font-family:'Font Awesome 5 Free';font-size:14px;color:var(--main-color);font-weight:400;margin:0 4px 0 0}
.rtl .entry-meta .entry-comments-link:before{margin:0 0 0 4px}
.entry-meta .entry-comments-link.show{display:block}
.entry-content-wrap{position:relative;float:left;width:100%;margin:25px 0 0}
#post-body{position:relative;text-align: justify;width:100%;font-family:var(--text-font);font-size:$(itempost.content.size);color:var(--post-text-color);line-height:1.6em;padding:0;margin:0;overflow: hidden;}
.post-body h1,.post-body h2,.post-body h3,.post-body h4,.post-body h5,.post-body h6{font-size: 20px;font-weight: normal;color: var(--main-color);text-transform: uppercase;margin: 10px 0;line-height:1.5em}
.post-body img{height:auto!important}
.rtl blockquote:before{left:unset;right:10px}
.post-body .responsive-video-wrap{position:relative;width:100%;padding:0;padding-top:56%}
.post-body .responsive-video-wrap iframe{position:absolute;top:0;left:0;width:100%;height:100%}
.post-body ul{padding:0 0 0 16px;margin:10px 0}
.rtl .post-body ul{padding:0 16px 0 0}
.post-body li{margin: 0;padding:0}
.post-body ul li,.post-body ol ul li{list-style:none}
.post-body ul li:before{display:inline-block;margin:0 5px 0 0}
.rtl .post-body ul li:before{margin:0 0 0 5px}
.post-body ol{counter-reset:ify;padding:0 0 0 16px;margin:10px 0}
.rtl .post-body ol{padding:0 16px 0 0}
.post-body ol > li{counter-increment:ify;list-style:none}
.post-body ol > li:before{display:inline-block;content:counters(ify,'.')'.';margin:0 5px 0 0}
.rtl .post-body ol > li:before{margin:0 0 0 5px}
.post-body u{text-decoration:none;}
.post-body strike{text-decoration:line-through}
.post-body sup{vertical-align:super}
.post-body a{color:var(--main-color);}
.post-body a:hover{text-decoration:none;}
.post-body a.button{display:inline-block;height:34px;background-color:var(--button-bg);font-family:var(--body-font);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;text-align:center;text-decoration:none;cursor:pointer;padding:0 20px;margin:0 6px 8px 0}
.rtl .post-body a.button{margin:0 0 8px 6px}
.post-body a.colored-button{color:#fff}
.post-body a.button:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.post-body a.colored-button:hover{background-color:var(--button-hover-bg)!important;color:var(--button-hover-color)!important}
.button:before{float:left;font-family:'Font Awesome 5 Free';font-weight:900;display:inline-block;margin:0 8px 0 0}
.rtl .button:before{float:right;margin:0 0 0 8px}
.button.preview:before{content:'\f06e'}
.button.download:before{content:'\f019'}
.button.link:before{content:'\f0c1'}
.button.cart:before{content:'\f07a'}
.button.info:before{content:'\f06a'}
.button.share:before{content:'\f1e0'}
.button.contact:before{content:'\f0e0';font-weight:400}
.alert-message{position:relative;display:block;padding:16px;border:1px solid var(--border-color);border-radius:var(--radius)}
.alert-message.alert-success{background-color:rgba(34,245,121,0.03);border:1px solid rgba(34,245,121,0.5)}
.alert-message.alert-info{background-color:rgba(55,153,220,0.03);border:1px solid rgba(55,153,220,0.5)}
.alert-message.alert-warning{background-color:rgba(185,139,61,0.03);border:1px solid rgba(185,139,61,0.5)}
.alert-message.alert-error{background-color:rgba(231,76,60,0.03);border:1px solid rgba(231,76,60,0.5)}
.alert-message:before{font-family:'Font Awesome 5 Free';font-size:16px;font-weight:900;display:inline-block;margin:0 5px 0 0}
.rtl .alert-message:before{margin:0 0 0 5px}
.alert-message.alert-success:before{content:'\f058';color:rgba(34,245,121,1)}
.alert-message.alert-info:before{content:'\f05a';color:rgba(55,153,220,1)}
.alert-message.alert-warning:before{content:'\f06a';color:rgba(185,139,61,1)}
.alert-message.alert-error:before{content:'\f057';color:rgba(231,76,60,1)}
.post-body table{width:100%;overflow-x:auto;text-align:left;margin:0;border-collapse:collapse;border:1px solid var(--border-color)}
.rtl .post-body table{text-align:right}
.post-body table td,.post-body table th{padding:6px 12px;border:1px solid var(--border-color)}
.post-body table thead th{color:var(--post-title-color);font-weight:700;vertical-align:bottom}
table.tr-caption-container,table.tr-caption-container td,table.tr-caption-container th{line-height:1;padding:0;border:0}
table.tr-caption-container td.tr-caption{font-size:13px;color:var(--meta-color);padding:6px 0 0}
.tocify-wrap{display:flex;width:100%;clear:both;margin:0}
.tocify-inner{position:relative;max-width:100%;background-color:var(--rgba-gray);display:flex;flex-direction:column;overflow:hidden;font-size:14px;color:var(--title-color);line-height:1.6em;border:0;border-radius:var(--radius)}
a.tocify-title{position:relative;height:40px;font-size:16px;color:var(--title-color);font-weight:700;display:flex;align-items:center;justify-content:space-between;padding:0 16px;margin:0}
.tocify-title-text{display:flex}
.tocify-title-text:before{content:'\f0cb';font-family:'Font Awesome 5 Free';font-size:14px;font-weight:900;margin:0 6px 0 0}
.rtl .tocify-title-text:after{margin:0 0 0 6px}
.tocify-title:after{content:'\f078';font-family:'Font Awesome 5 Free';font-size:12px;font-weight:900;margin:0 0 0 25px}
.rtl .tocify-title:after{margin:0 25px 0 0}
.tocify-title.is-expanded:after{content:'\f077'}
a.tocify-title:hover{text-decoration:none}
#tocify{display:none;padding:0 16px 10px;margin:0}
#tocify ol{padding:0 0 0 16px}
.rtl #tocify ol{padding:0 16px 0 0}
#tocify li{font-size:14px;margin:8px 0}
#tocify li a{color:var(--main-color)}
#tocify li a:hover{color:var(--main-color);}
.post-body .contact-form{display:table;font-family:var(--body-font)}
.contact-form .widget-title{display:none}
.contact-form .contact-form-name{width:calc(50% - 5px)}
.rtl .contact-form .contact-form-name{float:right}
.contact-form .contact-form-email{float:right;width:calc(50% - 5px)}
.rtl .contact-form .contact-form-email{float:left}
.post-body .google-auto-placed{margin:25px 0}
.post-footer{position:relative;float:left;width:100%;margin:0}
.entry-labels{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;margin:15px 0 0}
.entry-labels span,.entry-labels a{font-size:14px;color:var(--main-color);font-weight:400;margin:5px 6px 0 0}
.rtl .entry-labels span,.rtl .entry-labels a{margin:5px 0 0 6px}
.entry-labels span{color:var(--title-color);font-weight:700}
.entry-labels a:hover{text-decoration:none}
.entry-labels a:after{content:',';color:var(--meta-color)}
.entry-labels a:last-child:after{display:none}
.post-share{position:relative;float:left;width:100%;margin:20px 0 0}
ul.litespot-pro-share-links{display:flex;flex-wrap:wrap;align-items:flex-start}
.litespot-pro-share-links li{padding:0 5px 0 0}
.rtl .litespot-pro-share-links li{padding:0 0 0 5px}
.litespot-pro-share-links li a{display:flex;width:34px;height:34px;font-size:16px;color:#fff;font-weight:400;cursor:pointer;align-items:center;justify-content:center;margin:5px 0 0}
.litespot-pro-share-links li.has-span a{width:auto;justify-content:flex-start}
.litespot-pro-share-links li.has-span a:before{padding:0 10px}
.litespot-pro-share-links span{font-size:14px;line-height:1;padding:0 20px 0 10px;border-left:1px solid rgba(255,255,255,0.2)}
.rtl .litespot-pro-share-links span{padding:0 10px 0 20px;border-left:0;border-right:1px solid rgba(255,255,255,0.2)}
.litespot-pro-share-links li a:hover{opacity:.9}
.litespot-pro-share-links .show-hid a{background-color:var(--rgba-gray);font-size:14px;color:rgba(155,155,155,0.8)}
.litespot-pro-share-links .show-hid a:before{content:'\f067';font-family:'Font Awesome 5 Free';font-weight:900}
.show-hidden .show-hid a:before{content:'\f068'}
.litespot-pro-share-links li.reddit,.litespot-pro-share-links li.linkedin,.litespot-pro-share-links li.tumblr,.litespot-pro-share-links li.telegram{display:none}
.show-hidden li.reddit,.show-hidden li.linkedin,.show-hidden li.tumblr,.show-hidden li.telegram{display:inline-block}
.about-author{position:relative;float:left;width:100%;background-color:var(--widget-bg);display:flex;padding:16px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.about-author .author-avatar-wrap{width:60px;height:60px;margin:0 15px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .about-author .author-avatar-wrap{margin:0 0 0 15px}
.about-author .author-title{display:block;font-family:var(--title-font);font-size:16px;color:var(--title-color);font-weight:700;margin:0 0 10px}
.about-author .author-title a{color:var(--title-color)}
.about-author .author-title a:hover{color:var(--title-hover-color)}
.author-description{display:flex;flex-direction:column;flex:1}
.author-description .author-text{display:block;font-size:14px;color:var(--text-color);line-height:1.6em;font-weight:400}
.author-description .author-text br,.author-description .author-text a{display:none}
ul.author-links{display:flex;flex-wrap:wrap;padding:0}
.author-links li{margin:10px 12px 0 0}
.rtl .author-links li{margin:10px 0 0 12px}
.author-links li a{display:block;font-size:14px;color:var(--text-color);padding:0}
.author-links li a:hover{opacity:.9}
#litespot-pro-related-posts,#related-wrap .related-tag{display:none}
#related-wrap,.litespot-pro-related-content{position:relative;float:left;width:100%}
#related-wrap{margin:20px 0 0}
.litespot-pro-related-content .loader{height:200px}
.related-posts{display:grid;grid-template-columns:repeat(3,1fr);grid-gap:20px}
.related-item{position:relative;background-color:var(--post-card-bg);display:flex;flex-direction:column;overflow:hidden;border:1px solid var(--border-color);border-radius:var(--radius)}
.related-item .entry-image-wrap{width:100%;height:140px;border-radius:var(--radius) var(--radius) 0 0}
.related-item .entry-header{padding:13px 10px}
.related-item .entry-title{font-size:15px}
.litespot-pro-blog-post-comments{display:none;float:left;width:100%;margin:20px 0 0}
.comments-system-disqus,.comments-system-facebook{margin:20px 0 0}
.litespot-pro-blog-post-comments .fb_iframe_widget_fluid_desktop{float:left;display:block!important;width:calc(100% + 16px)!important;max-width:calc(100% + 16px)!important;margin:0 -8px}
.litespot-pro-blog-post-comments .fb_iframe_widget_fluid_desktop span,.litespot-pro-blog-post-comments .fb_iframe_widget_fluid_desktop iframe{float:left;display:block!important;width:100%!important}
#comments,#disqus_thread{position:relative;float:left;width:100%;display:block;clear:both}
#disqus_thread,.fb-comments{padding:0}
.comments-title,#comments h4#comment-post-message{display:none}
.comments-system-blogger .comments-title{display:block}
.comments .comments-content{float:left;width:100%;margin:0}
.comments .comment-content{display:block;font-family:var(--text-font);font-size:14px;color:var(--text-color);line-height:1.6em;margin:10px 0 0}
.comments .comment-content > a:hover{text-decoration:none}
.comment-thread .comment{position:relative;list-style:none;background-color:var(--widget-bg);padding:16px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.comment-thread .comment .comment{background-color:var(--rgba-gray);border:0}
.comment-thread ol{padding:0;margin:0}
.comment-thread .comment-replies ol{padding:0 0 4px}
.toplevel-thread ol > li:first-child{margin:0}
.toplevel-thread ol > li:first-child > .comment-block{padding-top:0;margin:0;border:0}
.comment-thread ol ol .comment:before{content:'\f3bf';position:absolute;left:-25px;top:-10px;font-family:'Font Awesome 5 Free';font-size:16px;color:var(--border-color);font-weight:700;transform:rotate(90deg);margin:0}
.rtl .comment-thread ol ol .comment:before{content:'\f3be';left:unset;right:-25px}
.comments .comment-replybox-single iframe{padding:0 0 0 48px;margin:10px 0 0}
.rtl .comments .comment-replybox-single iframe{padding:0 48px 0 0}
.comment-thread .avatar-image-container{position:absolute;top:16px;left:16px;width:35px;height:35px;overflow:hidden;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .comment-thread .avatar-image-container{left:auto;right:16px}
.avatar-image-container img{width:100%;height:100%}
.comments .comment-header{padding:0 0 0 48px}
.rtl .comments .comment-header{padding:0 48px 0 0}
.comments .comment-header .user{display:inline-block;font-family:var(--title-font);font-size:16px;color:var(--title-color);font-style:normal;font-weight:700;margin:0}
.comments .comment-header .user a{color:var(--title-color)}
.comments .comment-header .user a:hover{color:var(--title-hover-color)}
.comments .comment-header .icon.user{display:none}
.comments .comment-header .icon.blog-author{display:inline-block;font-size:13px;color:var(--main-color);font-weight:400;vertical-align:top;margin:-5px 0 0 4px}
.rtl .comments .comment-header .icon.blog-author{margin:-5px 4px 0 0}
.comments .comment-header .icon.blog-author:before{content:'\f058';font-family:'Font Awesome 5 Free';font-weight:400}
.comments .comment-header .datetime{display:block;margin:0}
.comment-header .datetime a{font-size:12px;color:var(--meta-color);font-weight:400;padding:0}
.comments .comment-actions{display:block;margin:10px 0 0}
.comments .comment-actions a{display:inline-block;font-size:14px;color:var(--main-color);font-weight:400;font-style:normal;padding:0;margin:0 15px 0 0}
.rtl .comments .comment-actions a{margin:0 0 0 15px}
.comments .comment-actions a:hover{color:var(--title-color)}
.item-control{display:none}
.loadmore.loaded a{display:inline-block;border-bottom:1px solid rgba(155,155,155,.51);text-decoration:none;margin-top:15px}
.comments .continue{display:none}
.comments .comment-replies{padding:0 0 0 48px}
.rtl .comments .comment-replies{padding:0 48px 0 0}
.thread-expanded .thread-count a,.loadmore{display:none}
.comments .footer{float:left;width:100%;font-size:13px;margin:0}
.comment-form{float:left;width:100%;margin:0}
p.comments-message{display:block;float:left;width:100%;font-size:13px;color:var(--meta-color);font-style:italic;margin:0 0 16px}
p.comments-message.no-new-comments{padding:0;margin:0;border:0}
p.comments-message > a{color:var(--main-color)}
p.comments-message > a:hover{color:var(--title-color)}
p.comments-message > em{color:#ff3f34;font-style:normal;margin:0 3px}
#comments[data-embed='false'] p.comments-message > i{color:var(--main-color);font-style:normal}
.comment-form > p{display:none}
.comment-content .responsive-video-wrap{position:relative;width:100%;padding:0;padding-top:56%}
.comment-content .responsive-video-wrap iframe{position:absolute;top:0;left:0;width:100%;height:100%}
.comments #top-ce.comment-replybox-thread,.comments.no-comments .comment-form{background-color:var(--widget-bg);padding:6px 16px;margin:20px 0 0;border:1px solid var(--border-color);border-radius:var(--radius)}
.comments.no-comments .comment-form{margin:0}
.comments #top-continue a{float:left;width:100%;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;text-align:center;padding:0;margin:20px 0 0;border-radius:var(--radius)}
.comments #top-continue a:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.post-nav{float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;font-size:14px;font-weight:400;margin:20px 0 0}
.post-nav span,.post-nav a{display:flex;align-items:center;color:var(--meta-color)}
.post-nav a:hover{color:var(--main-color)}
.post-nav span{color:var(--meta-color);cursor:no-drop;opacity:.65}
.post-nav-newer-link:before,.rtl .post-nav-older-link:after{content:'\f053';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:1px 4px 0 0}
.post-nav-older-link:after,.rtl .post-nav-newer-link:before{content:'\f054';font-family:'Font Awesome 5 Free';font-size:9px;font-weight:900;margin:1px 0 0 4px}
#custom-ads,#litespot-pro-post-footer-ads{position:relative;float:left;width:100%;opacity:0;visibility:hidden;padding:0;margin:0;border:0}
#before-ad,#after-ad{float:left;width:100%;margin:0}
#before-ad .widget > .widget-title,#after-ad .widget > .widget-title{display:block}
#before-ad .widget > .widget-title > .title,#after-ad .widget > .widget-title > .title{font-size:10px;color:var(--meta-color);font-weight:400;line-height:1;margin:0 0 6px}
#before-ad .widget,#after-ad .widget{width:100%;margin:0 0 15px}
#after-ad .widget{margin:15px 0 0}
#before-ad .widget-content,#after-ad .widget-content{position:relative;width:100%}
#litespot-pro-new-before-ad #before-ad,#litespot-pro-new-after-ad #after-ad{float:none;display:block;margin:0}
#litespot-pro-new-before-ad #before-ad .widget,#litespot-pro-new-after-ad #after-ad .widget{margin:0}
#post-footer-ads{position:relative;float:left;width:100%;padding:0;margin:20px 0 0}
#post-footer-ads .widget,#post-footer-ads .widget-content{float:left;width:100%}
#blog-pager{position:relative;float:left;width:100%;display:flex;justify-content:center;margin:20px 0 0}
#blog-pager.no-blog-posts{display:none}
#blog-pager .load-more{position:relative;display:flex;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);align-items:center;cursor:pointer;padding:0 20px}
#blog-pager #litespot-pro-load-more-link:after{content:'\f078';display:inline-block;font-family:'Font Awesome 5 Free';font-size:10px;font-weight:900;margin:0 0 0 4px}
.rtl #blog-pager #litespot-pro-load-more-link:after{margin:0 4px 0 0}
#blog-pager #litespot-pro-load-more-link:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
#blog-pager .no-more.show{display:flex;background-color:var(--rgba-gray);color:var(--meta-color);cursor:not-allowed}
#blog-pager .loading,#blog-pager .no-more{display:none}
#blog-pager .loading .loader{height:34px}
.sidebar{position:relative;float:left;width:100%;margin:0}
.sidebar > .widget{position:relative;float:left;width:100%;background-color:var(--widget-bg);margin:0 0 20px;border:1px solid var(--border-color);border-radius:var(--radius)}
.sidebar > .widget:last-child{margin:0}
.sidebar .title-wrap{padding:10px 16px;margin:0;border-bottom:1px solid var(--border-color)}
.sidebar .title-wrap .title:after{display:none}
.sidebar .widget-content{position:relative;float:left;width:100%;padding:12px}
.sidebar .widget.is-ad{background-color:transparent;border:0}
.sidebar .widget.is-ad > .widget-title{display:none}
.sidebar .widget.is-ad .widget-content{padding:0}
.sidebar ul.social-icons{display:grid;grid-template-columns:repeat(2,1fr);grid-gap:5px;margin:0}
.sidebar .social-icons li{display:block;margin:0}
.sidebar .social-icons a{position:relative;display:flex;height:34px;font-size:16px;color:#fff;font-weight:400;align-items:center}
.sidebar .social-icons a:before{padding:0 10px}
.sidebar .social-icons span{font-size:14px;line-height:1;padding:0 10px;border-left:1px solid rgba(255,255,255,0.2)}
.rtl .sidebar .social-icons span{border-left:0;border-right:1px solid rgba(255,255,255,0.2)}
.sidebar .social-icons a:hover{opacity:.9}
.sidebar .loader{height:180px}
.default-items{display:flex;flex-direction:column}
.default-items .cs{height:180px;overflow:hidden;border-radius:var(--radius)}
.default-items .default-inner{position:relative;width:100%;height:100%;display:flex;flex-direction:column}
.default-items .cs .entry-image-wrap{width:100%;height:100%;margin:0}
.default-items .entry-header{display:flex;flex-direction:column}
.default-items .cs .entry-title{font-size:18px}
.default-items .cs .entry-meta{flex-wrap:wrap}
.default-items .ds{display:flex;margin:20px 0 0}
.default-items .ds.item-0{margin:0}
.default-items .ds .entry-image-wrap{width:98px;height:65px;z-index:1;margin:0 12px 0 0;border-radius:var(--radius)}
.rtl .default-items .ds .entry-image-wrap{margin:0 0 0 12px}
.default-items .ds .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.7)}
.default-items .ds .entry-header{flex:1}
.default-items .ds .entry-title{font-size:14px}
.mini-items{position:relative;float:left;width:100%;display:grid;grid-template-columns:repeat(2,1fr);grid-gap:20px}
.mini-item{position:relative;display:flex;flex-direction:column}
.mini-item .entry-image-wrap{width:100%;height:82px;margin:0 0 8px;border-radius:var(--radius)}
.mini-item .entry-image-wrap.is-video:after{transform:translate(50%,-50%) scale(.85)}
.mini-item .entry-title{font-size:14px}
.cmm1-items{display:flex;flex-direction:column}
.cmm1-items .cmm1-item{position:relative;width:100%;padding:16px 0 0;margin:16px 0 0;border-top:1px solid var(--border-color)}
.cmm1-items .cmm1-item.item-0{padding:0;margin:0;border:0}
.cmm1-items .entry-inner{display:flex}
.cmm1-items .entry-image-wrap{width:35px;height:35px;z-index:1;margin:0 12px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .cmm1-items .entry-image-wrap{margin:0 0 0 12px}
.cmm1-items .entry-header{flex:1}
.cmm1-items .entry-title{font-size:14px}
.cmm1-items .entry-inner:hover .entry-title{color:var(--post-title-hover-color)}
.cmm1-items .cmm-snippet{font-size:12px;color:var(--text-color);margin:4px 0 0}
.FeaturedPost .featured-post{position:relative;width:100%;height:160px}
.FeaturedPost .fp-inner{position:relative;width:100%;height:100%;display:flex;flex-direction:column;z-index:11;overflow:hidden;border-radius:var(--radius)}
.featured-post .entry-image-wrap{width:100%;height:100%;z-index:1;margin:0}
.featured-post .entry-title{font-size:17px}
.featured-post .entry-meta{flex-wrap:wrap}
.section .list-style li{position:relative;display:block;font-size:14px;color:var(--title-color);font-weight:400}
.section .list-style li a{display:block;color:var(--title-color);padding:8px 0}
.section .list-style li a.has-count{display:flex;justify-content:space-between}
.section .list-style li:first-child a,.section .text-list li:first-child{padding:0 0 8px}
.section .list-style li:last-child a,.section .text-list li:last-child{padding:8px 0 0}
.section .list-style li a:hover{color:var(--title-hover-color)}
.section .list-style li a span{display:inline-block;color:var(--main-color)}
.section .text-list li{padding:8px 0}
.cloud-label ul{display:flex;flex-wrap:wrap;margin:-6px 0 0}
.cloud-label li{margin:6px 5px 0 0}
.rtl .cloud-label li{margin:6px 0 0 5px}
.cloud-label li a{display:flex;height:29px;color:var(--button-bg);font-size:14px;line-height:28px;font-weight:400;padding:0 10px;border:1px solid var(--button-bg)}
.cloud-label li a:hover{background-color:var(--button-bg);color:var(--button-color);border-color:var(--button-bg)}
.cloud-label .label-count{display:inline-block;margin:0 0 0 10px}
.rtl .cloud-label .label-count{margin:0 10px 0 0}
.search-widget .search-form{float:left;width:100%;display:flex;margin:0}
.search-widget .search-input{display:inline-block;flex:1;width:100%;height:34px;background-color:var(--rgba-gray);font-family:inherit;font-weight:400;font-size:14px;color:var(--text-color);padding:0 13px;margin:0;border:0;border-radius:var(--radius)}
.search-widget .search-input::placeholder{color:var(--text-color);opacity:.9}
.search-widget .search-input:focus{background-color:var(--widget-bg);box-shadow:0 1px 1px rgba(0,0,0,0.1),0 1px 3px rgba(0,0,0,0.2)}
.is-dark .search-widget .search-input:focus{background-color:var(--rgba-gray)}
.search-widget .search-action{display:inline-block;width:36px;height:34px;background-color:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;cursor:pointer;padding:0;margin:0 0 0 5px;border:0;border-radius:var(--radius)}
.rtl .search-widget .search-action{margin:0 5px 0 0}
.search-widget .search-action:before{display:block;content:'\f002';font-family:'Font Awesome 5 Free';font-weight:900}
.search-widget .search-action:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.Profile ul li{float:left;width:100%;padding:20px 0 0;margin:20px 0 0;border-top:1px solid var(--border-color)}
.Profile ul li:first-child{padding:0;margin:0;border:0}
.Profile .individual,.Profile .team-member{display:flex}
.Profile .profile-img{width:35px;height:35px;background-color:var(--rgba-gray);overflow:hidden;color:transparent!important;margin:0 12px 0 0;border-radius:50%;box-shadow:var(--avatar-shadow)}
.rtl .Profile .profile-img{margin:0 0 0 12px}
.Profile .profile-info{flex:1}
.Profile .profile-name{display:block;font-family:var(--title-font);font-size:15px;color:var(--title-color);font-weight:700;margin:0}
.Profile .profile-name:hover{color:var(--title-hover-color)}
.Profile .profile-link{display:block;font-size:12px;color:var(--meta-color);font-weight:400;margin:0}
.Profile .profile-link:hover{color:var(--main-color)}
.Text .widget-content{font-family:var(--text-font);font-size:14px;color:var(--text-color);margin:0}
.Image .image-caption{display:block;font-size:14px;color:var(--text-color);margin:6px 0 0}
.contact-form-widget form{font-family:inherit;font-weight:400}
.contact-form-name{float:left;width:100%;height:34px;background-color:var(--rgba-gray);font-family:inherit;font-size:14px;color:var(--text-color);line-height:34px;padding:0 15px;margin:0 0 10px;border:0;border-radius:var(--radius)}
.contact-form-email{float:left;width:100%;height:34px;background-color:var(--rgba-gray);font-family:inherit;font-size:14px;color:var(--text-color);line-height:34px;padding:0 15px;margin:0 0 10px;border:0;border-radius:var(--radius)}
.contact-form-email.error{border-color:var(--main-color)}
.contact-form-email-message{float:left;width:100%;background-color:var(--rgba-gray);font-family:inherit;font-size:14px;color:var(--text-color);padding:10px 15px;margin:0 0 10px;border:0;border-radius:var(--radius)}
.contact-form-email-message.error{border-color:var(--main-color)}
.contact-form-button-submit{float:left;width:100%;height:34px;background-color:var(--button-bg);font-family:inherit;font-size:14px;color:var(--button-color);font-weight:400;cursor:pointer;padding:0 20px;border:0;border-radius:var(--radius)}
.contact-form-button-submit:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.contact-form-widget p{margin:0}
.contact-form-widget p.contact-form-error-message-with-border,p.contact-form-success-message-with-border{float:left;width:100%;background-color:rgba(0,0,0,0);font-size:13px;color:#e74c3c;text-align:left;line-height:1;padding:0;margin:10px 0 0;border:0}
.contact-form-widget .contact-form-success-message-with-border{color:#27ae60}
.rtl .contact-form-error-message-with-border,.rtl .contact-form-success-message-with-border{text-align:right}
.contact-form-cross{cursor:pointer;margin:0 0 0 3px}
.rtl .contact-form-cross{margin:0 3px 0 0}
.contact-form-name::placeholder,.contact-form-email::placeholder,.contact-form-email-message::placeholder{color:var(--text-color);opacity:.9}
.contact-form-widget .cf-s:focus{background-color:var(--widget-bg);box-shadow:0 1px 1px rgba(0,0,0,0.1),0 1px 3px rgba(0,0,0,0.2)}
.is-dark .contact-form-widget .cf-s:focus{background-color:var(--rgba-gray)}
.Attribution a{font-size:14px;line-height:16px;display:block}
.Attribution a > svg{width:16px;height:16px;float:left;margin:0 4px 0 0}
.Attribution .copyright{font-size:12px;color:var(--meta-color);padding:0 20px;margin:3px 0 0}
#google_translate_element{position:relative;float:left;width:100%;padding:20px;margin:0}
.Stats .text-counter-wrapper{display:flex;align-items:center;font-size:20px;color:var(--title-color);font-weight:700;text-transform:uppercase;line-height:1;margin:0}
.Stats .text-counter-wrapper:before{content:'\f201';font-family:'Font Awesome 5 Free';font-size:18px;color:var(--main-color);font-weight:900;margin:1px 4px 0 0}
.rtl .Stats .text-counter-wrapper:before{margin:1px 0 0 4px}
.sidebar > .widget.ReportAbuse{display:block;padding:15px 20px;border:1px solid var(--border-color);border-radius:var(--radius)}
.ReportAbuse > h3{display:flex;float:left;width:100%;font-size:14px;font-weight:400;margin:0}
.ReportAbuse > h3:before{content:'\f071';font-family:'Font Awesome 5 Free';color:var(--title-color);font-weight:900;margin:0 4px 0 0}
.rtl .ReportAbuse > h3:before{margin:0 0 0 4px}
.ReportAbuse > h3 a:hover{text-decoration:none}
#footer-ads-wrap,.footer-ads .widget,.footer-ads .widget-content{position:relative;float:left;width:100%;margin:0}
.footer-ads .widget{margin:0 0 20px}
.footer-ads .widget > .widget-title{display:none}
#footer-wrapper{position:relative;float:left;width:100%;background-color:var(--footer-bg);color:var(--footer-color)}
#footer-wrapper .primary-footer{position:relative;float:left;width:100%;border-top:1px solid var(--border-color)}
.primary-footer.no-widget{display:none}
#litespot-pro-about-section{position:relative;float:left;width:100%;display:flex;flex-wrap:wrap;justify-content:space-between;padding:20px 0;margin:0}
.footer-info{flex:1}
.litespot-pro-about-section .Image{width:calc(100% - $(sidebar.width + 30px));display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between;padding:0}
.litespot-pro-about-section .footer-logo{padding:0 25px 0 0}
.rtl .litespot-pro-about-section .footer-logo{padding:0 0 0 25px}
.litespot-pro-about-section .footer-logo img{display:block;max-height:34px;margin:0}
.litespot-pro-about-section .Image .image-caption{font-size:14px;color:var(--footer-color);margin:0}
.litespot-pro-about-section .Image .image-caption a{color:var(--footer-color)}
.litespot-pro-about-section .Image .image-caption a:hover{color:var(--footer-hover-color)}
.litespot-pro-about-section .LinkList{width:$(sidebar.width);display:flex;align-items:center;justify-content:flex-end;margin:0}
.litespot-pro-about-section ul.social-icons{display:flex;flex-wrap:wrap}
.litespot-pro-about-section .social-icons li{margin:0 0 0 10px}
.rtl .litespot-pro-about-section .social-icons li{margin:0 10px 0 0}
.litespot-pro-about-section .social-icons li a{display:flex;width:34px;height:34px;background-color:var(--rgba-gray);font-size:16px;color:var(--footer-color);align-items:center;justify-content:center}
.litespot-pro-about-section .social-icons li a:hover{color:#fff}
.footerbar{position:relative;float:left;width:100%;background-color:var(--footerbar-bg);color:var(--footerbar-color);padding:20px 0;border-top:1px solid var(--border-color)}
.footerbar .container{display:flex;flex-wrap:wrap;justify-content:space-between}
.footerbar .footer-copyright{font-size:14px;font-weight:400;margin:0}
.footerbar .footer-copyright a{color:var(--footerbar-color)}
.footerbar .footer-copyright a:hover{color:var(--footerbar-hover-color)}
#footer-menu{position:relative;display:block;margin:0}
.footer-menu ul{display:flex;flex-wrap:wrap}
.footer-menu ul li a{font-size:14px;color:var(--footerbar-color);padding:0;margin:0 0 0 25px}
.rtl .footer-menu ul li a{margin:0 25px 0 0}
#footer-menu ul li a:hover{color:var(--footerbar-hover-color)}
#hidden-widgets-wrap,.hidden-widgets{display:none;visibility:hidden}
#back-top{display:none;position:fixed;bottom:20px;right:20px;width:34px;height:34px;background-color:var(--button-bg);cursor:pointer;overflow:hidden;font-size:15px;color:var(--button-color);text-align:center;line-height:34px;z-index:50;margin:0;transition:background .17s ease,color .17s ease}
.rtl #back-top{right:auto;left:20px}
#back-top:before{content:'\f077';position:relative;font-family:'Font Awesome 5 Free';font-weight:900}
#back-top:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.is-error #main-wrapper{width:100%}
.is-error #sidebar-wrapper{display:none}
.errorWrap{color:var(--title-color);text-align:center;padding:60px 0}
.errorWrap h3{font-size:160px;color:var(--title-color);line-height:1;margin:0 0 25px}
.errorWrap h4{font-size:27px;color:var(--title-color);margin:0 0 25px}
.errorWrap p{color:var(--text-color);font-size:14px;margin:0 0 15px}
.errorWrap a{display:inline-block;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;padding:0 30px;margin:15px 0 0;border-radius:var(--radius)}
.errorWrap a:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
.cookie-choices-info{display:none;visibility:hidden;opacity:0}
#litespot-pro-cookie-ify{display:none;position:fixed;bottom:20px;left:20px;width:300px;background-color:var(--cookie-bg);z-index:1020;padding:16px;visibility:hidden;opacity:0;border:1px solid var(--border-color);border-radius:var(--radius);box-shadow:0 1px 8px rgba(0,0,0,0.1);transition:all .35s ease,background 0s ease}
.rtl #litespot-pro-cookie-ify{left:unset;right:20px}
#litespot-pro-cookie-ify.is-visible{visibility:visible;opacity:1}
.litespot-pro-cookie-ify-content{display:block;font-size:14px;color:var(--cookie-color);margin:0 0 15px}
.litespot-pro-cookie-ify-content a{color:var(--cookie-color);text-decoration:none}
.litespot-pro-cookie-ify-content a:hover{color:var(--main-color)}
#litespot-pro-cookie-ify-accept{display:inline-block;height:34px;background-color:var(--button-bg);font-size:14px;color:var(--button-color);font-weight:400;line-height:34px;padding:0 20px}
#litespot-pro-cookie-ify-accept:hover{background-color:var(--button-hover-bg);color:var(--button-hover-color)}
ins.adsbygoogle-noablate[data-anchor-shown="true"]{z-index:990!important}
a.ads-here{position:relative;display:flex;align-items:center;justify-content:center;height:78px;background-color:var(--rgba-gray);font-size:15px;color:rgba(155,155,155,0.5);font-weight:500;font-style:italic;border:1px solid var(--border-color);border-radius:var(--radius)}
.is-dark a.ads-here{background-color:var(--widget-bg)}
.sidebar a.ads-here{height:250px}
a.ads-here:hover{color:rgba(155,155,155,0.65)}
@media only screen and (max-width: $(row.width + 60px)) {
#outer-wrapper,.is-boxed #outer-wrapper,.is-boxed .header-header{width:100%;max-width:100%;margin:0}
.row-x1{width:100%}
#header-wrapper .container,#header-ads-wrap .container,#ticker-wrapper .container,#featured-wrapper .container,#content-wrapper .container,#footer-ads-wrap .container,#footer-wrapper .container{padding:0 20px}
}
@media only screen and (max-width: 980px) {
#header-wrapper .container,#header-ads-wrap .container,#ticker-wrapper .container,#featured-wrapper .container,#content-wrapper .container,#footer-ads-wrap .container,#footer-wrapper .container{padding:0 16px}
#header-wrapper .container{padding:0}
.mobile-menu-toggle{display:flex}
.header-items{flex-wrap:nowrap}
#litespot-pro-main-nav{display:none}
#slide-menu,.overlay{display:block}
.flex-left,.main-logo{padding:0!important}
.flex-right{padding:0 16px}
.flex-right,.rtl .flex-right{position:relative;top:unset;left:unset;right:unset}
#main-search-wrap{width:100%;padding:0 16px}
.nav-active .overlay{visibility:visible;opacity:1}
.nav-active #back-top{opacity:0!important}
#content-wrapper > .container,.is-left #content-wrapper > .container{flex-direction:column!important;justify-content:flex-start}
#main-wrapper,#sidebar-wrapper{width:100%}
#sidebar-wrapper{margin:20px 0 0}
.sidebar ul.social-icons{grid-template-columns:repeat(4,1fr)}
.mini-items{grid-template-columns:repeat(4,1fr)}
.FeaturedPost .featured-post{height:200px}
.featured-post .entry-title{font-size:19px}
#litespot-pro-about-section{flex-wrap:wrap;flex-direction:column}
.litespot-pro-about-section .Image{width:100%;flex-direction:column;justify-content:center;text-align:center}
.litespot-pro-about-section .footer-logo{padding:0!important}
.footer-info{text-align:center;margin:20px 0 0}
.litespot-pro-about-section .LinkList{width:100%;justify-content:center;margin:10px 0 0}
.litespot-pro-about-section ul.social-icons{justify-content:center}
.litespot-pro-about-section .social-icons li{margin:10px 5px 0!important}
#litespot-pro-cookie-ify{left:16px;bottom:16px}
.rtl #litespot-pro-cookie-ify{left:unset;right:16px}
#back-top{right:16px;bottom:16px}
.rtl #back-top{left:16px;right:unset}
}
@media only screen and (max-width: 880px) {
.footerbar{height:auto;line-height:inherit;padding:25px 0;margin:0}
.footerbar .container{flex-direction:column;justify-content:center}
.footerbar .footer-copyright,#footer-menu{width:100%;text-align:center;margin:0}
#footer-menu{padding:5px 0 0}
.footer-menu ul{justify-content:center}
.footer-menu ul li a{display:block;margin:5px 10px 0!important}
}
@media only screen and (max-width: 680px) {
html.is-dark{--post-card-bg:var(--rgba-gray)}
#outer-wrapper{background-color:var(--outer-mobile-bg)}
.header-ads .widget{margin:16px 0 0}
#ticker-wrapper .container{padding:0}
#ticker .widget{flex-direction:column;align-items:initial;margin:16px 0 0;border-width:1px 0;border-radius:0}
.ticker .widget-title{padding:0;margin:0 0 5px}
.ticker .widget-content{height:initial}
.ticker .loader{margin:4px 0 0}
.ticker .ticker-item.active{position:relative}
.ticker-item .entry-title{height:initial;line-height:1.3em}
.ticker-item .entry-title a{white-space:initial;text-overflow:initial}
#featured-wrapper .container{padding:0}
#featured .widget{background-color:var(--widget-bg);padding:20px 16px;margin:16px 0 0;border:1px solid var(--border-color);border-width:1px 0}
.featured-items{grid-template-columns:1fr;grid-gap:16px}
#content-wrapper{padding:16px 0}
#content-wrapper .container{padding:0}
.content-section .widget{background-color:var(--widget-bg);padding:20px 16px;margin:0 0 16px;border:1px solid var(--border-color);border-width:1px 0}
.content-section .widget.is-ad{background-color:transparent;padding:0 16px;border:0}
.is-home #main-wrapper.has-cs2 #main{margin:0 0 16px}
.block-items{grid-template-columns:1fr;grid-gap:16px}
.block-right .block-item{margin:16px 0 0}
.block-left .entry-image-wrap{height:200px}
.grid-items,.video-items,.related-posts{grid-template-columns:repeat(2,1fr);grid-gap:16px}
.list-item{flex-direction:column;justify-content:flex-start;overflow:hidden;padding:0}
.list-item .entry-image-wrap{width:100%;height:200px;margin:0!important;border-radius:var(--radius) var(--radius) 0 0}
.list-item .entry-header{padding:13px 16px 16px}
.blog-posts-wrap{background-color:var(--widget-bg);padding:20px 16px;border:1px solid var(--border-color);border-width:1px 0}
.index-post{flex-direction:column;justify-content:flex-start;overflow:hidden;padding:0}
.index-post .entry-image-wrap{width:100%;height:200px;margin:0!important;border-radius:var(--radius) var(--radius) 0 0}
.index-post .entry-header{padding:13px 16px 16px}
#blog-pager{margin:20px 0 4px}
.item-post-inner{background-color:var(--widget-bg);padding:20px 16px;border:1px solid var(--border-color);border-width:1px 0}
.entry-content-wrap{margin:20px 0 0}
.item-post h1.entry-title{font-size:33px}
.post-body table{display:block}
.litespot-pro-share-links a.twitter span{display:none}
.litespot-pro-share-links li.has-span a.twitter{width:34px;justify-content:center}
.litespot-pro-share-links li.has-span a.twitter:before{background-color:transparent;padding:0}
#before-ad .widget{margin:0 0 20px}
#after-ad .widget{margin:20px 0 0}
.entry-labels,.post-share{margin:15px 0 0}
.about-author{padding:20px 16px;margin:16px 0 0;border-width:1px 0;border-radius:0}
#related-wrap{background-color:var(--widget-bg);padding:20px 16px;margin:16px 0 0;border:1px solid var(--border-color);border-width:1px 0}
#post-footer-ads{padding:0 16px;margin:16px 0 0}
.litespot-pro-blog-post-comments{background-color:var(--widget-bg);padding:20px 16px;margin:16px 0 0;border:1px solid var(--border-color);border-width:1px 0}
.post-nav{padding:0 16px;margin:16px 0 0}
#custom-ads{padding:0 16px}
#sidebar-wrapper{margin:16px 0 0}
.sidebar > .widget{padding:20px 16px;margin:0 0 16px;border-width:1px 0;border-radius:0}
.sidebar .widget.is-ad{padding:0 16px}
.sidebar .title-wrap{padding:0;margin:0 0 16px;border:0}
.sidebar .widget-content{padding:0}
.sidebar ul.social-icons{grid-template-columns:repeat(2,1fr)}
.mini-items{grid-template-columns:repeat(2,1fr);column-gap:16px}
.mini-item .entry-image-wrap{height:140px}
.mini-item .entry-title{font-size:15px}
.footer-ads .widget{margin:0 0 16px}
#litespot-pro-about-section{padding:26px 0 30px}
.errorWrap{padding:0 16px 30px}
.errorWrap h3{font-size:130px}
.errorWrap h4{line-height:initial}
#litespot-pro-cookie-ify{right:0!important;left:0!important;bottom:0;width:100%;padding:20px 16px;margin:0;border-radius:0;transform:translate3d(0,50%,0);transition:all .5s ease,background 0s ease}
#litespot-pro-cookie-ify.is-visible{transform:translate3d(0,0,0)}
a.ads-here{height:65px}
.sidebar a.ads-here{height:200px}
}
@media only screen and (max-width: 480px) {
.grid-item .entry-image-wrap,.video-item .entry-image-wrap,.related-item .entry-image-wrap{height:110px}
#post-body{font-size:$(itempost.content.size + 1px)}
.author-description .author-text,.comments .comment-content{font-size:15px}
.item-post h1.entry-title{font-size:31px}
.mini-item .entry-image-wrap{height:110px}
}
@media only screen and (max-width: 380px) {
#featured .widget-content{min-height:180px}
.featured-item{height:180px}
.block-left .entry-image-wrap{height:180px}
.list-item .entry-image-wrap{height:180px}
.grid-item .entry-image-wrap,.video-item .entry-image-wrap,.related-item .entry-image-wrap{height:95px}
.grid-item .entry-title,.video-item .entry-title,.related-item .entry-title{font-size:14px}
.index-post .entry-image-wrap{height:180px}
.item-post h1.entry-title{font-size:27px}
.item-post .entry-meta .align-right{display:none}
.tocify-inner{min-width:100%}
.litespot-pro-share-links span{display:none}
.litespot-pro-share-links li.has-span a{width:34px;justify-content:center}
.litespot-pro-share-links li.has-span a:before{background-color:transparent;padding:0}
.mini-item .entry-image-wrap{height:95px}
.mini-item .entry-title{font-size:14px}
.FeaturedPost .featured-post{height:180px}
}
@media only screen and (max-width: 340px) {
#slide-menu{width:100%}
.errorWrap h3{font-size:110px}
.errorWrap h4{font-size:27px}
}
/* jPLAYER */
.jp-controls button{
	speak: none;
	font-style: normal;
	font-weight: normal;
	font-variant: normal;
	text-transform: none;
	line-height: 1;
	-webkit-font-smoothing: antialiased;
}
.jp-audio-stream :focus,
.jp-video :focus {
 outline:0
}
.jp-audio button::-moz-focus-inner,
.jp-audio-stream button::-moz-focus-inner,
.jp-video button::-moz-focus-inner {
 border:0
}
.jp-audio,
.jp-audio-stream,
.jp-video {
 font-size:16px;
 font-family:Verdana,Arial,sans-serif;
 line-height:1.6;
 color:#666;
 background: #2f3038;
}
.jp-audio {
 width:100%;
}
.jp-audio-stream {
 width:182px
}
.jp-video-270p {
 width:480px
}
.jp-video-360p {
 width:640px
}
.jp-video-full {
 width:480px;
 height:270px;
 position:static!important;
 position:relative
}
.jp-video-full div div {
 z-index:1000
}
.jp-video-full .jp-jplayer {
 top:0;
 left:0;
 position:fixed!important;
 position:relative;
 overflow:hidden
}
.jp-video-full .jp-gui {
 position:fixed!important;
 position:static;
 top:0;
 left:0;
 width:100%;
 height:100%;
 z-index:1001
}
.jp-video-full .jp-interface {
 position:absolute!important;
 position:relative;
 bottom:0;
 left:0
}
.jp-interface {
 position:relative;
 background-color:#2f3038;
 width:100%
}
.jp-audio .jp-interface,
.jp-audio-stream .jp-interface {
 display: block;
 float: left;
 width: 100%;
}
.jp-video .jp-interface {
 border-top:1px solid #009be3
}
.jp-controls-holder {
 clear:both;
 width:440px;
 margin:0 auto;
 position:relative;
 overflow:hidden;
 top:-8px
}
.jp-interface .jp-controls {
 margin:0;
 padding:0;
 overflow:hidden
}
.jp-audio .jp-controls {
 margin: 15px 20px;
 display: inline-block;
 float: left;
}
.jp-audio-stream .jp-controls {
 position:absolute;
 top:20px;
 left:20px;
 width:142px
}
.jp-video .jp-type-single .jp-controls {
 width:78px;
 margin-left:200px
}
.jp-video .jp-type-playlist .jp-controls {
 width:134px;
 margin-left:172px
}
.jp-video .jp-controls {
 float:left
}
.jp-controls button {
 display: inline-block;
 float:left;
 overflow:hidden;
 border:none;
 cursor:pointer;
}
.jp-play:before,.jp-state-playing .jp-play:before {
  position: absolute;
  color: #fff;
  font-weight: 900;
  z-index: 5;
  display: flex;
  transform: translate(50%,-50%);
}
.fa-forward:before,.fa-backward:before{
  position: absolute;
  color: #fff;
  font-weight: 900;
  z-index: 5;
  display: flex;
  transform: translate(40%,-50%);
}
.jp-play:before {
	content: '\f04b';
}
.jp-state-playing .jp-play:before {
	content: '\f04c' !important;
}
.fa-forward:before{
	content: '\f04e';
}
.fa-backward:before{
	content: '\f04a';
  }
.jp-state-playing .jp-play {
 background:var(--main-color);
 color:#fff;
 border-color: var(--main-color);
}
.jp-next,
.jp-previous,
.jp-stop {
}
.jp-stop {
}

.jp-previous {
 background:;
}
.jp-progress {
 background-color:#ddd;
}
.jp-audio .jp-progress {
 height:10px;
 border-radius: 3px;
}
.jp-audio .jp-type-single .jp-progress {
 left:110px;
 width:186px
}
.jp-audio .jp-type-playlist .jp-progress {
 width: 160px;
 margin-top: 28px;
 display: inline-block;
 margin-left: 5px;
}
.jp-video .jp-progress {
 top:0;
 left:0;
 width:100%;
 height:10px
}
.jp-seek-bar {
 width:0;
 height:100%;
 cursor:pointer
}
.jp-play-bar {
 background:var(--main-color);
 width:0;
 height:100%;
 border-radius: 0 3px 3px 0;
}
.jp-seeking-bg {background:url(https://lh6.googleusercontent.com/-y8vIsuSoEuI/YIlcyRhiBdI/AAAAAAAAAUY/q4usaVYhS3ca-9giVf6GNfl_A6DIUnTGgCLcBGAsYHQ/s0/jplayer.blue.monday.seeking.gif);
border-radius: 0 3px 3px 0;
}
.jp-state-no-volume .jp-volume-controls {
 display:none
}
.jp-volume-controls {
 position:absolute;
 top:16px;
 left:280px;
 width:200px;
}
.jp-audio-stream .jp-volume-controls {
 left:70px
}
.jp-video .jp-volume-controls {
 top:12px;
 left:50px
}
.jp-volume-controls button {
 display:block;
 position:absolute;
 overflow:hidden;
 border:none;
 cursor:pointer;
 background: #2f3038;
}
.jp-mute,
.jp-volume-max {
 width:28;
 height:28;
}
.jp-volume-max {
 left:70px;
}

.jp-volume-bar {
 position:absolute;
 overflow:hidden;
 background:rgba(183, 197, 205, 0.66);
 top:11px;
 left:22px;
 width:46px;
 height:5px;
 cursor:pointer
}
.jp-volume-bar-value {
 width:0;
 height:5px;
 background: var(--main-color);
}
.jp-audio .jp-time-holder {
}
.jp-audio .jp-type-single .jp-time-holder {
 left:110px;
 width:186px
}
.jp-audio .jp-type-playlist .jp-time-holder {
 display: inline-block;
}
.jp-current-time,
.jp-duration {
 width:60px;
 font-size:.80em;
 font-style:oblique
}
.jp-current-time {
    display: inline;
    cursor: default;
    margin: 0 20px;
}
.jp-duration {
 display:inline;
 text-align:right;
}
.jp-video .jp-current-time {
 margin-left:20px
}
.jp-video .jp-duration {
 margin-right:20px
}
.jp-details {
 font-weight:700;
 text-align:center;
 cursor:default
}
.jp-details,
.jp-playlist {
 width:100%;
 background-color:#2f3038;
 border-top:;
 max-height: 250px;
 overflow-y: scroll;
}
.jp-type-playlist .jp-details,
.jp-type-single .jp-details {
 border-top:none
}
.jp-details .jp-title {
 margin:0;
 padding:5px 20px;
 font-size:.72em;
 font-weight:700
}
.jp-playlist ul {
 list-style-type:none;
 margin:0;
 padding:0;
 font-size:14px;
}
.jp-playlist li {
 padding:;
}
.jp-playlist li div {
 display:inline
}
div.jp-type-playlist div.jp-playlist li:last-child {
 border-bottom:none
}
div.jp-type-playlist div.jp-playlist li.jp-playlist-current {
 list-style-type:;
 list-style-position:;
 padding-left:;
 background: var(--main-color) !important;
 color: ;
}
div.jp-type-playlist div.jp-playlist a {
 color:#ddd;
 text-decoration:none;
 display: block;
 padding: 10px 15px;
 white-space: nowrap;
 overflow: hidden;
}
div.jp-type-playlist div.jp-playlist a.jp-playlist-current,
div.jp-type-playlist div.jp-playlist a:hover {
 color:#fff;
}
div.jp-type-playlist div.jp-playlist a.jp-playlist-item-remove {
 float:right;
 display:inline;
 text-align:right;
 margin-right:10px;
 font-weight:700;
 color:#666
}
div.jp-type-playlist div.jp-playlist a.jp-playlist-item-remove:hover {
 color:var(--main-color);
}
div.jp-type-playlist div.jp-playlist span.jp-free-media {
 float:right;
 display:inline;
 text-align:right;
 margin-right:10px
}
div.jp-type-playlist div.jp-playlist span.jp-free-media a {
 color:#666
}
div.jp-type-playlist div.jp-playlist span.jp-free-media a:hover {
 color:var(--main-color);
}
span.jp-artist {
 font-size:.8em;
 color:#666
}
.jp-video-play {
 width:100%;
 overflow:hidden;
 cursor:pointer;
 background-color:transparent
}
.jp-video-270p .jp-video-play {
 margin-top:-270px;
 height:270px
}
.jp-video-360p .jp-video-play {
 margin-top:-360px;
 height:360px
}
.jp-video-full .jp-video-play {
 height:100%
}
.jp-video-play-icon {
 position:relative;
 display:block;
 width:112px;
 height:100px;
 margin-left:-56px;
 margin-top:-50px;
 left:50%;
 top:50%;
 border:none;
 cursor:pointer
}
.jp-jplayer,
.jp-jplayer audio {
 width:0;
 height:0
}
.jp-jplayer {
 background-color:#000
}
.jp-toggles {
 padding:0;
 margin:0 auto;
 overflow:hidden
}
.jp-audio .jp-type-single .jp-toggles {
 width:25px
}
.jp-audio .jp-type-playlist .jp-toggles {
 width:55px;
 margin:0;
 position:absolute;
 left:325px;
 top:50px
}
.jp-video .jp-toggles {
 position:absolute;
 right:16px;
 margin:10px 0 0;
 width:100px
}
.jp-toggles button {
 display:block;
 float:left;
 width:25px;
 height:18px;
 text-indent:-9999px;
 line-height:100%;
 border:none;
 cursor:pointer
}
.jp-no-solution {
 padding:5px;
 font-size:.8em;
 background-color:#eee;
 border:2px solid #009be3;
 color:#000;
 display:none
}
.jp-no-solution a {
 color:#000
}
.jp-no-solution span {
 font-size:1em;
 display:block;
 text-align:center;
 font-weight:700
}
.jp-playlist li:nth-child(2n+1) {
    background: #26262d;
}
.jp-controls button {
    background: #2f3038;
}
.jp-controls button:hover {
  background: var(--main-color);
  color: #fff;
}
.jp-controls button {
  width: 35px;
  height: 35px;
  border-radius: 3px;
  margin-right: 10px;
  border: 1px solid #444;
}

.jp-playlist-item:focus{
	outline:none!important;
}
.jp-playlist::-webkit-scrollbar {
    width: 10px;    
}
.jp-playlist::-webkit-scrollbar-track {
   -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
   background-color: #2f3038;
}
.jp-playlist::-webkit-scrollbar-thumb {
   background-color: #686971;
 }
.jp-playlist::-webkit-scrollbar-thumb:hover {
   background-color: #5e5f66;
 }
.dangnghe {
    display: inline;
    margin-right: 5px;
}

alert.alert-success.showlisten {
    margin: 5px 0;
    padding: 5px 10px;
    float: left;
    width: 100%;
}
.alert-success {
    border-radius:var(--radius);
	background-color: var(--rgba-gray);
}
.alert {
	margin: 5px 0 0;
    padding: 10px 12px;
    border: 1px solid transparent;
 	clear:both;
	border: 1px solid var(--border-color);
}

.showlisten button.close {
    margin: 0;
}
* {
    outline: none!important;
}
.righttime {
    float: right;
    margin-bottom: 2px;
}
.settime {
    display: block;
    float: left;
    width: 100%;
}
#zingaudio_container {
    float: left;
    display: block;
	margin-bottom:5px;
}
span.timex {
    display: block;
    padding: 10px 15px;
    border-bottom: 1px solid #ddd;
    cursor: pointer;
}
span.timex:hover {
    background: #ddd;
}
.showtime {
    display: inline-block;
}
.hengio .dropdown-menu{
right:0!important; 
left: unset!important;
top:33px!important;
}
.rightunset {
    right:unset !important;
	left: unset!important;
	top:33px!important;
}
.jp-playlist-item-download {
    float: right;
    display: inline!important;
    text-align: right;
    margin-right: 10px;
    font-weight: 700;
    color: #666;
}
button.close {
    padding: 0;
    cursor: pointer;
    background: transparent;
    border: 0;
    -webkit-appearance: none;
}
button.close {float: right;font-size: 21px;font-weight: 700;line-height: 1;color: var(--post-text-color);opacity: .2;filter: alpha(opacity = 20)}
.close: hover, .close: focus {color: #000;text-decoration:none;cursor:pointer;opacity:.5;filter:alpha(opacity= 50)}
.fa-download{display:none}	
.btn-default{background-color: var(--rgba-gray);border: 1px solid var(--border-color);padding: 6px 8px;}
.btn-default:hover{color:#fff;background-color:var(--main-color);}
/* DISABLE SELECT */
.post-body,.post-body img{-webkit-user-select:none;-khtml-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}
 /* PRE - CODE */
.post-body pre,code,pre.code-box{background-color: var(--rgba-gray);border: 1px solid var(--border-color);font-family:Monospace;border-radius:var(--radius)}
pre{overflow:auto;word-wrap:normal;position:relative;height:100%;max-height:350px;white-space: pre-wrap;line-height:1.4em;padding:12px;margin:10px 0;}
pre>code{white-space:pre;word-wrap:initial;display:block}
pre>code td{border:0}
code{display: inline-block; position: relative;margin: 3px;padding: 2px 5px;}
table td{-webkit-user-select:all;-moz-user-select:all;-ms-user-select:all;user-select:all}
pre:hover::-webkit-scrollbar{width:5px}
pre::-webkit-scrollbar{width:0}
pre::-webkit-scrollbar-thumb{background:#ddd;border-radius:10px}
pre::-webkit-scrollbar-thumb:active{background:#bbb}
pre,code,blockquote{-webkit-user-select:all;-moz-user-select:all;-ms-user-select:all;user-select:all}
blockquote{position:relative;background-color: var(--rgba-gray);border: 1px solid var(--border-color);font-style:normal;padding:16px 20px;margin:5px 0;border-radius:var(--radius)}
blockquote:before{position:absolute;left:10px;top:10px;content:'\f10e';font-family:'Font Awesome 5 Free';font-size:33px;font-style:normal;font-weight:900;color:var(--title-color);line-height:1;opacity:.05;margin:0}
.btn-sm{font-size:16px;line-height:1.6em;color: var(--post-text-color);margin:5px 0}
.btn-sm:hover{cursor:pointer}
]]></b:skin>
</b:if>
<b:if cond='data:view.isLayoutMode'>
<b:template-skin><![CDATA[
html,body#layout #outer-wrapper,body#layout .row{width:auto;padding:0}
body#layout{position:relative;width:auto;max-width:100%;background-color:#f9f9f9;padding:95px 5px 0;margin:0}
body#layout:before{content:'Doc Truyen Online v1.0';position:absolute;top:0;left:5px;right:5px;height:95px;font-family:Verdana,sans-serif;font-size:23px;color:#0F1618;line-height:95px;text-align:center}
body#layout div.section{display:block;background-color:#f1f1f1!important;margin:0 5px 10px!important;padding:16px 16px 18px!important;border-color:#e5e5e5}
body#layout .no-items.section{display:block}
body#layout .section h4{font-size:14px;color:#0F1618;text-transform:uppercase;margin:0}
body#layout .section h4:after{text-transform:initial;color:#656565;font-weight:400}
body#layout .add_widget a{color:#3c97ef!important}
body#layout .widget-wrap3{overflow:hidden}
body#layout .widget-content{width:auto;max-width:none;max-height:none;margin:0;border:1px solid #e5e5e5;border-left:0}
body#layout .locked-widget .widget-content{border-left:1px solid #3c97ef}
body#layout .locked-widget .widget-content:hover{border-left-color:#00b140}
body#layout .widget .widget-content a.editlink{border-radius:2px}
body#layout .visibility .editlink{background:#3c97ef url(https://lh6.googleusercontent.com/-iQoCOwqjB-w/Wy1bDznOM4I/AAAAAAAACGA/8BUOPStr0sk5oud9hWpHBQTrmkeJDoAvACK4BGAYYCw/s18-c/mode_edit_w600_24dp.png) no-repeat center!important}
body#layout .visibility .editlink:hover{background-color:#00b140!important}
body#layout .draggable-widget .widget-wrap2{background:#3c97ef url(https://lh6.googleusercontent.com/-yTAuT5aZ1EY/Wy1eEeo4SbI/AAAAAAAACGM/FxOTPwL-Ch0_lyZxLRzhv2EWHINOmCjWACK4BGAYYCw/s22/draggable.png) no-repeat 4px 50%!important}
body#layout .draggable-widget .widget-wrap1:hover .widget-wrap2{background-color:#00b140!important}
body#layout .visibility .layout-widget-state.visible{background-image:url(https://lh6.googleusercontent.com/-qicweZaCb7I/XR_IGBqqGfI/AAAAAAAABS0/MIpI_COKj6MBkeN9FEJhqL96WYnYfGjngCK4BGAYYCw/s1600/visibility_c3_600_24dp.png)!important}
body#layout .visibility .layout-widget-state.not-visible{background-image:url(https://lh6.googleusercontent.com/-tqL3-mrEM7A/XR_H_P3mFZI/AAAAAAAABSs/4PO1g3CDQbse_mJYzwn-60OQoYMFcq1FQCK4BGAYYCw/s1600/visibility_off_c3_600_24dp.png)!important;opacity:1}
body#layout div.layout-widget-description{display:none;font-size:11px;line-height:1.2em}
body#layout #theme-options,body#layout #main-menu .widget{display:block!important}
body#layout div.ify-panel{background-color:#edf4ff!important;overflow:hidden!important;border-color:#cdd4ef}
body#layout .ify-panel .widget{float:left;width:32.66%;margin-right:1%}
body#layout .ify-panel .widget-content{border-color:#cdd4ef!important}
body#layout .ify-panel .HTML{margin-right:0}
body#layout .ify-panel div.layout-widget-description,body#layout .flex-right,body#layout #nav-search-wrap{display:none}
body#layout .flex-left{display:flex}
body#layout .main-logo,body#layout .litespot-pro-main-nav{width:50%}
body#layout #content-wrapper{padding:0;margin:0}
body#layout #content-wrapper > .container{display:flex;margin:0}
body#layout #main-wrapper{width:67%;padding:0}
body#layout div.content-section.section,body#layout div.main-ads.section{background-color:#edf4ff!important;border-color:#d9dff3}
body#layout #sidebar-wrapper{width:33%;padding:0}
body#layout #custom-ads{display:flex}
body#layout #custom-ads .section{width:50%}
body#layout #litespot-pro-about-section{overflow:hidden!important}
body#layout #litespot-pro-about-section .widget{float:left;width:49.5%;margin-right:1%}
body#layout #litespot-pro-about-section .LinkList{margin-right:0}
body#layout .footerbar .container{display:flex}
body#layout #footer-menu,body#layout #footer-copyright{width:50%}
body#layout .section > h4:after{font-size:12px}
body#layout #ify-panel > h4:after{content:' - Custom No Image, Date Format, Month Names and More.'}
body#layout #main-logo > h4:after{content:' - Recommended Height (34px)'}
body#layout #litespot-pro-main-nav > h4:after{content:' - With SubLinks and Mega Menu'}
body#layout #header-ads > h4:after{content:' - by Custom HTML, Adsense or Image'}
body#layout #ticker > h4:after,body#layout #featured > h4:after{content:' - by Popular Posts, Most Recents or Label'}
body#layout .content-section > h4:after{content:' - by Most Recents or Label or AD Gadget (Adsense, HTML)'}
body#layout #main > h4:after{content:' - Default Blog Posts, AdSense In-Feed, Comments and More'}
body#layout #litespot-pro-main-before-ad > h4:after{content:' - Before Post Content (Post Page)'}
body#layout #litespot-pro-main-after-ad > h4:after{content:' - After Post Content (Post Page)'}
body#layout #litespot-pro-related-posts > h4:after{content:' - Advanced Related Posts'}
body#layout #litespot-pro-post-footer-ads > h4:after{content:' - After Related Posts (Post Page)'}
body#layout #sidebar > h4:after{content:' - on All Pages'}
body#layout:after{content:'Doc Truyen Online v1.0';display:block;font-family:Verdana,sans-serif;font-size:20px;color:#555;line-height:1;text-align:center;visibility:visible;padding:20px 0}
body#layout #footer-ads > h4:after{content:' - by Custom HTML, Adsense or Image'}
body#layout #litespot-pro-about-section > h4:after{content:' - Site Logo, Description and Social Icons'}
body#layout #footer-copyright > h4:after{content:' - Custom Credits'}
body#layout #footer-menu > h4:after{content:' - Footer Links'}
body#layout #litespot-pro-cookie-ify-section > h4:after{content:' - Advanced Cookie Consent Plugin'}
body#layout #hidden-widgets{display:none!important}
]]></b:template-skin>
</b:if>
<b:if cond='data:widgets.AdSense.first or data:blog.adsenseClientId'>
  <!-- Google AdSense -->
  <script async='async' src='//pagead2.googlesyndication.com/pagead/js/adsbygoogle.js'/>
</b:if>
<!--  <b:if cond='data:blog.analyticsAccountNumber'>
  <b:include data='blog' name='google-analytics'/>
</b:if> -->
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-R9VDQKWWMK"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-R9VDQKWWMK');
</script>
<b:defaultmarkups>
  <b:defaultmarkup type='Common'>
    <b:includable id='theme-dark-mode'>
      <b:class cond='data:skin.vars.darkmode == &quot;1px&quot;' name='is-dark'/>
    </b:includable>
    <b:includable id='customOpenGraphMetaData'>
      <!-- Metadata for Open Graph protocol. See http://ogp.me/. -->
      <meta expr:content='data:blog.localeUnderscoreDelimited' property='og:locale'/>
      <b:if cond='data:view.isHomepage'>
        <meta content='website' property='og:type'/>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <meta content='article' property='og:type'/>
      </b:if>
      <b:if cond='data:view.isMultipleItems and not data:view.isHomepage'>
        <meta content='object' property='og:type'/>
      </b:if>
      <meta expr:content='data:view.title.escaped' property='og:title'/>
      <meta expr:content='data:blog.url.canonical' property='og:url'/>
      <meta expr:content='data:view.description.escaped' property='og:description'/>
      <meta expr:content='data:blog.title.escaped' property='og:site_name'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:content='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='meta' property='og:image'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:content='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='meta' property='twitter:image'/>
      <b:if cond='data:view.featuredImage'>
        <meta expr:content='data:view.featuredImage resizeImage 1600' property='og:image'/>
        <meta expr:content='data:view.featuredImage resizeImage 1600' name='twitter:image'/>
      </b:if>
      <meta content='summary_large_image' name='twitter:card'/>
      <meta expr:content='data:view.title.escaped' name='twitter:title'/>
      <meta expr:content='data:blog.url.canonical' name='twitter:domain'/>
      <meta expr:content='data:view.description.escaped' name='twitter:description'/>
    </b:includable>
    <b:includable id='theme-head'>
      <meta expr:content='&quot;text/html; charset=&quot; + data:blog.encoding' http-equiv='Content-Type'/>
      <meta content='width=device-width, initial-scale=1, minimum-scale=1, maximum-scale=1, user-scalable=yes' name='viewport'/>
      <b:if cond='data:blog.pageType == &quot;error_page&quot;'>
<title>404 - Không tìm thấy trang! - <data:blog.title/></title>
<meta content='2;/' http-equiv='refresh'/>
</b:if>
<b:if cond='data:blog.pageType != &quot;item&quot;'>
<b:if cond='data:blog.searchQuery'>
<title>Kết quả tìm kiếm về <data:blog.searchQuery/></title></b:if>
<b:if cond='data:blog.pageType == &quot;archive&quot;'>
  <title><data:blog.pageName/> - <data:blog.title/></title>
<meta expr:content='&quot;danh mục bài viết &quot; + data:blog.pageName + &quot; Tìm hiểu thêm vui lòng truy cập&quot;' name='description'/><b:else/>
<b:if cond='data:blog.pageType == &quot;static_page&quot;'>
<title><data:blog.pageName/> </title><b:else/><b:if cond='data:blog.searchLabel'>
<title><data:blog.pageName/> - <data:blog.title/></title>
<meta expr:content='&quot;Chuyên mục &quot; + data:blog.pageName + &quot; của TruyenMaHot.Com&quot;' name='description'/>
<b:else/>
<title><data:blog.pageTitle/></title></b:if></b:if></b:if>
<meta content='Đọc Truyện Online,Truyện Ma Hot,Audio truyện hay,audio truyen full,audio truyện full,truyện audio,truyện tiên hiệp full,truyện kiếm hiệp full,truyện xuyên không full,truyen tien hiep audio,truyen kiem hiep audio,truyen audio tien hiep,audio truyen hay,audio truyện,truyen ngon tinh,truyện ngôn tình,ngôn tình audio' name='keywords'/>
<b:else/>
<title><data:blog.pageName/></title>
<meta expr:content='data:blog.pageName + &quot;, Đọc Truyện Online,Truyện Ma Hot,Audio truyện hay,audio truyen full,audio truyện full,truyện audio,truyện tiên hiệp full,truyện kiếm hiệp full,truyện xuyên không full,truyen tien hiep audio,truyen kiem hiep audio,truyen audio tien hiep,audio truyen hay,audio truyện,truyen ngon tinh,truyện ngôn tình,ngôn tình audio&quot;' name='keywords'/>
</b:if>
    <link href='//fonts.gstatic.com' rel='dns-prefetch'/>
    <link href='//cdnjs.cloudflare.com' rel='dns-prefetch'/>
    <link href='//1.bp.blogspot.com' rel='dns-prefetch'/>
    <link href='//2.bp.blogspot.com' rel='dns-prefetch'/>
    <link href='//3.bp.blogspot.com' rel='dns-prefetch'/>
    <link href='//4.bp.blogspot.com' rel='dns-prefetch'/>
    <link href='//www.blogger.com' rel='dns-prefetch'/>
	<link href='//lh5.googleusercontent.com' rel='dns-prefetch'/>
	<link href='//lh6.googleusercontent.com' rel='dns-prefetch'/>
	<link href='//github.com' rel='dns-prefetch'/>
	<link href='//apis.google.com' rel='dns-prefetch'/>
	<link href='//www.google-analytics.com' rel='dns-prefetch'/>
	<link href='//pagead2.googlesyndication.com' rel='dns-prefetch'/>
	<link href='//googleads.g.doubleclick.net' rel='dns-prefetch'/>
	<link href='//www.gstatic.com' rel='dns-prefetch'/>
	<link href='//www.googletagservices.com' rel='dns-prefetch'/>
	<link href='//tpc.googlesyndication.com' rel='dns-prefetch'/>
	<link href='//syndication.twitter.com' rel='dns-prefetch'/>
	<link href='//fonts.gstatic.com' rel='dns-prefetch'/>
	<link href='//raw.githack.com' rel='dns-prefetch'/>
	<link href='//tpc.googlesyndication.com' rel='dns-prefetch'/>
	<link href='//i.ytimg.com' rel='dns-prefetch'/>
	<link href='//i3.ytimg.com' rel='dns-prefetch'/>
	<link href='//img.youtube.com' rel='dns-prefetch'/>
	<link href='//www.youtube.com' rel='dns-prefetch'/>
	<link href='//www.googletagmanager.com' rel='dns-prefetch'/>
	<link href='//adservice.google.com' rel='dns-prefetch'/>
	<link href='//archive.org' rel='dns-prefetch'/>
	<link href='//us.archive.org' rel='dns-prefetch'/>
	<link href='//docs.google.com' rel='dns-prefetch'/>
      <meta content='blogger' name='generator'/>
      <link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
      <meta expr:content='data:skin.vars.main_color' name='theme-color'/>
      <b:if cond='data:blog.adultContent'>
        <meta content='adult' name='rating'/>
      </b:if>
      <link expr:href='data:view.url.canonical' rel='canonical'/>
      <meta expr:content='data:view.description.escaped' name='description'/>
      <b:tag cond='data:view.isMultipleItems and data:widgets.Blog.first.posts[0].featuredImage' expr:href='data:widgets.Blog.first.posts[0].featuredImage resizeImage 1600' name='link' rel='image_src'/>
      <b:tag cond='data:view.isSingleItem and data:view.featuredImage' expr:href='data:view.featuredImage resizeImage 1600' name='link' rel='image_src'/>
      <b:include name='customOpenGraphMetaData'/>
      <data:blog.feedLinks/><data:blog.meTag/>
      <b:if cond='data:view.isHomepage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;WebSite&quot;,&quot;name&quot;:&quot;<data:view.title.escaped/>&quot;,&quot;url&quot;:&quot;<data:view.url.canonical/>&quot;,&quot;potentialAction&quot;:{&quot;@type&quot;:&quot;SearchAction&quot;,&quot;target&quot;:&quot;<data:view.url.canonical/>search?q={search_term_string}&quot;,&quot;query-input&quot;:&quot;required name=search_term_string&quot;}}</script>
      </b:if>
      <!-- Font Awesome Free 5.15.2 -->
      <b:tag href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.2/css/fontawesome.min.css' name='link' rel='stylesheet'/>
    </b:includable>
    <b:includable id='theme-body-class'>
      <b:class cond='data:view.isHomepage' name='is-home'/>
      <b:class cond='data:view.isMultipleItems' name='is-multiple'/>
      <b:class cond='data:view.isSingleItem' name='is-single'/>
      <b:class cond='data:view.isPage' name='is-page'/>
      <b:class cond='data:view.isPost' name='is-post'/>
      <b:class cond='data:view.isError' name='is-multiple is-error'/>
      <b:class cond='data:blog.isMobileRequest' name='is-mobile'/>
      <b:class cond='data:skin.vars.boxed == &quot;1px&quot;' name='is-boxed'/>
      <b:class cond='data:skin.vars.sidebar == &quot;1px&quot;' name='is-left'/>
    </b:includable>
    <b:includable id='theme-custom-lang'>
      <b:switch var='data:message'>
        <b:case value='prevPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Previous Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Anterior<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Postagem Anterior<b:else/><data:messages.newer/></b:if>
        <b:case value='nextPost'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Next Post<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Artículo Siguiente<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Próxima Postagem<b:else/><data:messages.older/></b:if>
        <b:case value='loadMorePosts'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>Load More<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Carga Más<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Carregar Mais<b:else/><data:messages.loadMorePosts/></b:if>
        <b:case value='noMorePosts'/><b:if cond='data:blog.locale.language == &quot;en&quot;'>That is All<b:elseif cond='data:blog.locale.language == &quot;es&quot;'/>Eso es Todo<b:elseif cond='data:blog.locale.language == &quot;pt&quot;'/>Isso é Tudo<b:else/><data:messages.noResultsFound/></b:if>
      </b:switch>
    </b:includable>
    <b:includable id='widget-title'>
      <b:if cond='data:title == &quot;{ads}&quot;'>
        <b:class name='is-ad'/>
        <b:elseif cond='data:widget.type == &quot;AdSense&quot;'/>
        <b:class name='is-ad'/>
      </b:if>
      <b:if cond='data:defaultTitle or data:title'>
        <b:if cond='(data:title != &quot;{ads}&quot;)'>
          <b:if cond='data:widget.sectionId not in [&quot;ify-panel&quot;,&quot;main-logo&quot;,&quot;litespot-pro-main-nav&quot;,&quot;header-ads&quot;,&quot;featured&quot;,&quot;footer-ads&quot;,&quot;litespot-pro-post-footer-ads&quot;,&quot;litespot-pro-about-section&quot;,&quot;footer-copyright&quot;,&quot;footer-menu&quot;]'>
            <div expr:class='data:widget.sectionId in [&quot;content-section-1&quot;,&quot;content-section-2&quot;,&quot;sidebar&quot;] ? &quot;widget-title title-wrap&quot; : &quot;widget-title&quot;'><h3 class='title'><data:title/></h3></div>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='linklist-content'>
      <b:if cond='data:widget.sectionId == &quot;litespot-pro-main-nav&quot;'>
        <ul id='litespot-pro-main-nav-menu' role='menubar'>
          <b:loop values='data:links' var='link'>
            <li><b:if cond='data:link.target contains &quot;getContent&quot;'><b:class name='has-sub mega-menu'/><a expr:data-shortcode='data:link.target' href='#' role='menuitem'><data:link.name/></a><b:else/><a expr:href='data:link.target in [&quot;{homepage}&quot;] ? data:blog.homepageUrl.canonical : data:link.target' role='menuitem'><data:link.name/></a></b:if></li>
          </b:loop>
        </ul>
        <b:elseif cond='data:widget.sectionId in [&quot;sidebar&quot;,&quot;litespot-pro-about-section&quot;]'/>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;litespot-pro-about-section&quot;]' name='div'>
          <b:if cond='data:links any l =&gt; l.name in [&quot;blogger&quot;,&quot;facebook&quot;,&quot;facebook-f&quot;,&quot;twitter&quot;,&quot;rss&quot;,&quot;youtube&quot;,&quot;skype&quot;,&quot;stumbleupon&quot;,&quot;tumblr&quot;,&quot;vk&quot;,&quot;stack-overflow&quot;,&quot;github&quot;,&quot;linkedin&quot;,&quot;dribbble&quot;,&quot;soundcloud&quot;,&quot;behance&quot;,&quot;digg&quot;,&quot;instagram&quot;,&quot;pinterest&quot;,&quot;pinterest-p&quot;,&quot;twitch&quot;,&quot;delicious&quot;,&quot;codepen&quot;,&quot;amazon&quot;,&quot;reddit&quot;,&quot;whatsapp&quot;,&quot;messenger&quot;,&quot;microsoft&quot;,&quot;telegram&quot;,&quot;discord&quot;,&quot;apple&quot;,&quot;email&quot;,&quot;external-link&quot;]'>
            <b:if cond='data:widget.sectionId == &quot;sidebar&quot;'>
              <ul class='social-icons social social-bg'>
                <b:loop index='i' values='data:links' var='link'>
                  <li expr:class='data:link.name + &quot; link-&quot; + data:i'><a expr:alt='data:link.name' expr:class='data:link.name + &quot; btn&quot;' expr:href='data:link.target' expr:title='data:link.name' rel='noopener noreferrer' target='_blank'/></li>
                </b:loop>
              </ul>
              <b:else/>
              <ul class='social-icons social social-bg-hover'>
                <b:loop index='i' values='data:links' var='link'>
                  <li expr:class='data:link.name + &quot; link-&quot; + data:i'><a expr:alt='data:link.name' expr:class='data:link.name + &quot; btn&quot;' expr:href='data:link.target' expr:title='data:link.name' rel='noopener noreferrer' target='_blank'/></li>
                </b:loop>
              </ul>
            </b:if>
            <b:else/>
            <ul class='link-list list-style'>
              <b:loop values='data:links' var='link'>
                <li><a expr:href='data:link.target'><data:link.name/></a></li>
              </b:loop>
            </ul>
          </b:if>
        </b:tag>
        <b:else/>
        <b:tag class='widget-content' cond='data:widget.sectionId not in [&quot;footer-menu&quot;]' name='div'>
          <ul expr:class='data:widget.sectionId == &quot;footer-menu&quot; ? &quot;link-list&quot; : &quot;link-list list-style&quot;'>
            <b:loop values='data:links' var='link'>
              <li><a expr:href='data:link.target'><data:link.name/></a></li>
            </b:loop>
          </ul>
        </b:tag>
      </b:if>
    </b:includable>
    <b:includable id='html-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:if cond='data:content != &quot;&quot;'>
          <b:tag name='script' type='text/javascript'>
            <b:with expr:value='data:content' var='option'>
              <b:if cond='data:option.viewAllText'>var viewAllText = &quot;<data:option.viewAllText/>&quot;;</b:if>
              <b:if cond='data:option.dateFormat'>var dateFormat = &quot;<data:option.dateFormat/>&quot;;</b:if>
              <b:if cond='data:option.months'>
                var monthNames = [&quot;<data:option.months.jan/>&quot;,&quot;<data:option.months.feb/>&quot;,&quot;<data:option.months.mar/>&quot;,&quot;<data:option.months.apr/>&quot;,&quot;<data:option.months.may/>&quot;,&quot;<data:option.months.jun/>&quot;,&quot;<data:option.months.jul/>&quot;,&quot;<data:option.months.aug/>&quot;,&quot;<data:option.months.sep/>&quot;,&quot;<data:option.months.oct/>&quot;,&quot;<data:option.months.nov/>&quot;,&quot;<data:option.months.dec/>&quot;];
              </b:if>
            </b:with>
          </b:tag>
        </b:if>
      <b:elseif cond='data:widget.sectionId == &quot;litespot-pro-related-posts&quot;'/>
        <b:with value='data:title ? &quot;$title={&quot; + data:title + &quot;} &quot; : &quot;&quot;' var='relatedTitle'>
          <b:attr expr:value='data:relatedTitle + (data:content contains &quot;results&quot; ? data:content : &quot;&quot;)' name='data-shortcode'/>
        </b:with>
        <b:else/>
        <b:if cond='data:content contains &quot;getContent&quot; and data:widget.sectionId in [&quot;ticker&quot;,&quot;featured&quot;,&quot;content-section-1&quot;,&quot;content-section-2&quot;]'>
          <b:class name='is-visible'/>
        </b:if>
        <b:include name='widget-title'/>
        <div class='widget-content'>
          <b:if cond='data:content contains &quot;getContent&quot; and data:widget.sectionId in [&quot;sidebar&quot;,&quot;ticker&quot;,&quot;featured&quot;,&quot;content-section-1&quot;,&quot;content-section-2&quot;]'>
            <b:attr expr:value='data:content' name='data-shortcode'/>
            <b:else/>
            <data:content/>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='textlist-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:loop index='i' values='data:items' var='item'>
          <b:if cond='data:i == 0'>
            <script async='async' crossorigin='anonymous' defer='defer' expr:src='data:item'/>
          </b:if>
        </b:loop>
        <b:else/>
        <div class='widget-content'>
          <ul class='text-list list-style'>
            <b:loop values='data:items' var='item'>
              <li><data:item/></li>
            </b:loop>
          </ul>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='image-content'>
      <b:if cond='data:widget.sectionId == &quot;ify-panel&quot;'>
        <b:tag name='script' type='text/javascript'>var noThumbnail = &quot;<b:eval expr='resizeImage(data:sourceUrl, 72, &quot;1:1&quot;)'/>&quot;;</b:tag>
        <b:elseif cond='data:widget.sectionId == &quot;litespot-pro-about-section&quot;'/>
        <a class='footer-logo custom-image' expr:href='data:link'>
          <img expr:alt='data:blog.title' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl'/>
        </a>
        <b:if cond='data:caption'>
          <div class='footer-info'>
            <p class='image-caption excerpt'><data:caption/></p>
          </div>
        </b:if>
        <b:else/>
        <div class='widget-content'>
          <div class='custom-image'>
            <b:tag cond='data:link' expr:href='data:link' name='a'>
              <img expr:alt='data:blog.title' expr:id='data:widget.instanceId + &quot;_img&quot;' expr:src='data:sourceUrl'/>
            </b:tag>
          </div>
          <b:if cond='data:caption'>
            <p class='image-caption excerpt'><data:caption/></p>
          </b:if>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='text-content'>
       <b:if cond='data:widget.sectionId == &quot;footer-copyright&quot;'>
        <data:content/>
        <b:elseif cond='data:widget.sectionId == &quot;litespot-pro-cookie-ify-section&quot;'/>
        <b:attr expr:value='data:title' name='data-shortcode'/>
        <p class='litespot-pro-cookie-ify-content excerpt'><data:content/></p>
        <a class='btn' expr:title='data:messages.ok' href='javascript:;' id='litespot-pro-cookie-ify-accept' role='button'><data:messages.ok/></a>
        <b:else/>
        <b:include name='widget-title'/>
        <div class='widget-content excerpt'>
          <data:content/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='popular-content'>
      <div expr:class='&quot;default-item ds item-&quot;+data:i'>
        <a class='entry-image-wrap' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
        <div class='entry-header'>
          <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
          <b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><span class='entry-time mi'><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></div></b:if>
        </div>
      </div>
    </b:includable>
    <b:includable id='contact-form-content'>
      <div class='widget-content contact-form-widget'>
        <form name='contact-form'>
          <input class='contact-form-name cf-s' expr:ariby='data:contactFormNameMsg' expr:id='data:widget.instanceId + &quot;_contact-form-name&quot;' expr:placeholder='data:contactFormNameMsg' name='name' size='30' type='text' value=''/>
          <input class='contact-form-email cf-s' expr:ariby='data:contactFormEmailMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email&quot;' expr:placeholder='data:contactFormEmailMsg + &quot; *&quot;' name='email' size='30' type='text' value=''/>
          <textarea class='contact-form-email-message cf-s' cols='25' expr:ariby='data:contactFormMessageMsg + &quot; *&quot;' expr:id='data:widget.instanceId + &quot;_contact-form-email-message&quot;' expr:placeholder='data:contactFormMessageMsg + &quot; *&quot;' name='email-message' rows='5'/>
          <input class='contact-form-button btn contact-form-button-submit' expr:id='data:widget.instanceId + &quot;_contact-form-submit&quot;' expr:value='data:contactFormSendMsg' type='button'/>
          <p class='contact-form-error-message' expr:id='data:widget.instanceId + &quot;_contact-form-error-message&quot;'/>
          <p class='contact-form-success-message' expr:id='data:widget.instanceId + &quot;_contact-form-success-message&quot;'/>
        </form>
      </div>
    </b:includable>
    <b:includable id='theme-options-js'>
      <b:if cond='data:skin.vars.fixedmenu == &quot;0px&quot; or (data:skin.vars.fixedsidebar == &quot;0px&quot;) or (data:skin.vars.darkmode == &quot;1px&quot;) or (data:skin.vars.userdarkmode == &quot;0px&quot;)'>
      <!-- Theme Options JS -->
      <b:tag name='script' type='text/javascript'><b:if cond='data:skin.vars.fixedmenu == &quot;0px&quot;'>var fixedMenu=false;</b:if><b:if cond='data:skin.vars.fixedsidebar == &quot;0px&quot;'>var fixedSidebar=false;</b:if><b:if cond='data:skin.vars.darkmode == &quot;1px&quot;'>var darkMode=true;</b:if><b:if cond='data:skin.vars.userdarkmode == &quot;0px&quot;'>var userDarkMode=false;</b:if></b:tag>
      </b:if>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Header'>
    <b:includable id='main' var='this'>
      <b:tag class='mobile-menu-toggle' href='javascript:;' name='a' role='button' title='Menu'/>
      <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
      <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='title'/>
    </b:includable>
    <b:includable id='image'>
      <a class='logo-img' expr:href='data:blog.homepageUrl.canonical'>
        <img expr:alt='data:blog.title.escaped' expr:data-height='data:height' expr:data-width='data:width' expr:src='data:image' expr:title='data:blog.title.escaped'/>
        <b:if cond='data:view.isMultipleItems'><b:if cond='data:widget.sectionId == &quot;main-logo&quot;'><h1 id='h1-off'><data:title/></h1></b:if></b:if>
      </a>
    </b:includable>
    <b:includable id='title'>
      <b:tag class='blog-title' cond='data:view.isMultipleItems' name='h1'>
        <b:tag class='blog-title' cond='!data:view.isMultipleItems' name='span'>
          <b:tag expr:href='data:blog.homepageUrl.canonical' name='a'>
            <data:title/>
          </b:tag>
        </b:tag>
      </b:tag>
    </b:includable>
    <b:includable id='behindImageStyle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='description'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='LinkList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='TextList'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='textlist-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='HTML'>
    <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Text'>
    <b:includable id='main'>
      <b:include name='text-content'/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Blog'>
    <b:includable id='main' var='this'>
      <b:tag class='blog-posts-wrap' cond='data:view.isMultipleItems' name='div'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <div class='blog-posts hfeed'>
          <b:class cond='data:view.isMultipleItems' name='index-post-wrap'/>
          <b:class cond='data:view.isSingleItem' name='item-post-wrap'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='postCommentsAndAd'/>
          </b:loop>
        </div>
      </b:tag>
      <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
      <b:include name='feedLinks'/>
      <b:include name='exportBlogContent'/>
    </b:includable>
    <b:includable id='exportBlogContent'>
      <b:tag name='script' type='text/javascript'>
      var exportify = {
      noTitle: &quot;<data:messages.noTitle/>&quot;,
      viewAll: &quot;<data:messages.viewAll/>&quot;,
      postAuthor: <b:eval expr='data:allBylineItems.author ? &quot;true&quot; : &quot;false&quot;'/>,
      postAuthorLabel: &quot;<b:eval expr='data:allBylineItems.author.label ? data:allBylineItems.author.label : &quot;&quot;'/>&quot;,
      postDate: <b:eval expr='data:allBylineItems.timestamp ? &quot;true&quot; : &quot;false&quot;'/>,
      postDateLabel: &quot;<b:eval expr='data:allBylineItems.timestamp.label ? data:allBylineItems.timestamp.label : &quot;&quot;'/>&quot;
      }
      </b:tag>
    </b:includable>
    <b:includable id='aboutPostAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
    <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination on Index -->
      <div class='blog-pager' id='blog-pager'>
        <b:class cond='data:posts.empty' name='no-blog-posts'/>
        <b:if cond='data:olderPageUrl'>
          <a class='blog-pager-older-link load-more btn' expr:data-load='data:olderPageUrl.canonical' href='javascript:;' id='litespot-pro-load-more-link'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='theme-custom-lang'/></a>
          <span class='loading'><div class='loader'/></span>
          <span class='no-more load-more btn'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
          <b:else/>
          <span class='no-more load-more btn show'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='backLinks' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='blogPostsTitle'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <div class='title-wrap bp-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='wt-l' href='/search'><data:messages.viewAll/></a></div>
      </b:if>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentAuthorAvatar'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentDeleteIcon' var='comment'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='90px' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <script type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </script>
      </div>
    </b:includable>
    <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=soho&quot;' id='comment-editor-src' rel='noopener noreferrer' title='Comment Form Link'/>
    </b:includable>
    <b:includable id='commentItem' var='comment'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentList' var='comments'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentPicker' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='comments' var='post'>
      <a name='comments'/>
      <b:include name='commentsTitle'/>
      <section class='comments threaded' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
    <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <div class='title-wrap comments-title'><h3 class='title'><b:if cond='data:post.numberOfComments != 0'><data:post.numberOfComments/> <data:messages.comments/><b:else/><data:messages.postAComment/></b:if></h3></div>
    </b:includable>
    <b:includable id='defaultAdUnit'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='feedLinks'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='feedLinksBody' var='links'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
            </div>
            <b:if cond='data:allBylineItems.comments'>
              <div class='align-right'>
                <b:include cond='data:allBylineItems.comments' data='post' name='postCommentsLink'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='homePageLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='iframeComments' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postHeader'/>
        <b:include data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
    <b:includable id='inlineAd' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include data='post' name='postMeta'/>
      <div class='item-post-inner'>
        <div class='entry-header blog-entry-header p-eh'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap'>
          <b:include data='post' name='postBody'/>
          <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
          <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
        </div>
      </div>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
    </b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-older-link' expr:href='data:olderPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-older-link&quot;'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
    <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author mi'><b:if cond='data:view.isPost'><span class='author-avatar-wrap'><span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://lh6.googleusercontent.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/></span></b:if><b:if cond='data:allBylineItems.author.label'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
    <b:includable id='postBody' var='post'> 
      <!-- Ads before post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-main-before-ad&quot;' id='before-ad' name='div'/></b:if>
      <!-- Post Body Entry Content-->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
      <!-- Ads after post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-main-after-ad&quot;' id='after-ad' name='div'/></b:if>
    </b:includable>
    <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 125 }'/></p></b:includable>
    <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <b:if cond='data:view.isPost'>
        <b:if cond='data:skin.vars.breadcrumb == &quot;1px&quot;'><nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl'><data:messages.home/></a><b:if cond='data:post.labels'><em class='delimiter'/><a class='label' expr:href='data:post.labels.first.url'><data:post.labels.first.name/></a></b:if></nav></b:if>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
      <b:if cond='data:view.isPage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
    </b:includable>
    <b:includable id='postCategory' var='post'>
      <!-- Post Label -->
      <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
    </b:includable>
    <b:includable id='postCommentsAndAd' var='post'>
      <!-- In-Feed Ads -->
      <b:include cond='data:view.isMultipleItems and not data:view.search.label and not data:view.search.query and not data:view.isArchive' data='post' name='inlineAd'/>
      <article class='blog-post hentry'>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post post-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post'/>
        <b:include data='post' name='post'/>
      </article>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='litespot-pro-blog-post-comments' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='threadedCommentsDisqus'/>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
    <b:includable id='postCommentsLink'>
      <b:if cond='data:skin.vars.cmm_count == &quot;1px&quot;'>
        <!-- Post Comments Count -->
        <span class='entry-comments-link'><data:post.numberOfComments/></span>
      </b:if>
    </b:includable>
    <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a class='entry-image-wrap' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
    </b:includable>
    <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <b:tag class='post-footer' cond='data:post.author.aboutMe or (data:widgets.HTML any w =&gt; w.sectionId == &quot;litespot-pro-related-posts&quot;) or (data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-post-footer-ads&quot;)' name='footer'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;litespot-pro-related-posts&quot;' data='post' name='relatedPosts'/>
        <b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-post-footer-ads&quot;' id='post-footer-ads' name='div'/>
      </b:tag>
    </b:includable>
    <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author'>
        <div class='author-avatar-wrap'>
          <span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://lh6.googleusercontent.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/>
        </div>
        <div class='author-description'>
          <span class='author-title'><b:tag cond='data:post.author.profileUrl' expr:alt='data:post.author.name' expr:href='data:post.author.profileUrl' name='a' rel='noopener noreferrer' target='_blank'><data:post.author.name/></b:tag></span>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
    <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isSingleItem' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
    <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
    <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link' expr:href='data:label.url' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}}</script>
      </b:if>
    </b:includable>
    <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons' var='post'>
      <!-- Post ShareButtons -->
      <div class='post-share'>
        <ul class='litespot-pro-share-links social social-bg'>
          <li class='facebook has-span'><a class='facebook btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='twitter btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='whatsapp btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsEscaped + &quot; | &quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='WhatsApp'/></li>
          <li class='pinterest-p'><a class='pinterest btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.pinterest.com/pin/create/button/?url=&quot; + data:post.url.canonical + &quot;&amp;media=&quot; + data:post.featuredImage + &quot;&amp;description=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Pinterest'/></li>
          <li class='reddit'><a class='reddit btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://reddit.com/submit?url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Reddit'/></li>
          <li class='linkedin'><a class='linkedin btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='LinkedIn'/></li>
          <li class='tumblr'><a class='tumblr btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.tumblr.com/share/link?url=&quot; + data:post.url.canonical + &quot;&amp;name=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Tumblr'/></li>
          <li class='telegram'><a class='telegram btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://telegram.me/share/url?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Telegram'/></li>
          <li class='email'><a class='email btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;mailto:?subject=&quot; + data:post.title.jsEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Email'/></li>
          <li class='show-hid'><a class='btn' expr:title='data:messages.showMore' href='javascript:;' rel='nofollow'/></li>
        </ul>
      </div>
    </b:includable>
    <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time mi'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
    <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a class='entry-title-link' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
    <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-newer-link' expr:href='data:newerPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-newer-link&quot;'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
    <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div id='related-wrap'>
        <div class='title-wrap related-title'>
          <span class='title'><span class='t-text'><data:messages.youMayLikeThesePosts/></span></span>
        </div>
        <div class='litespot-pro-related-content'>
          <b:if cond='data:post.labels'>
            <div class='related-tag' expr:data-label='data:post.labels.first.name'/>
            <b:else/>
            <div class='related-tag' data-label='recent'/>
          </b:if>
        </div> 
      </div>  
    </b:includable>
    <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span>
            <b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span></b:if></div>
      </b:if><b:tag name='script' id='MM' src="//www.truyenmahot.com"/><b:if cond='data:view.isArchive'>
        <div class='queryMessage'><b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span>
            <b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentForm' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentJs' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedComments' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='threadedCommentsDisqus' var='post'>
    <script type='text/javascript'>
        var disqus_shortname = &quot;templateify-comments&quot;;
        var disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        if (!disqus_blogger_current_url.length) {
          disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
        }
        var disqus_blogger_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
        var disqus_blogger_canonical_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
      </script>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='PopularPosts'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;ticker&quot;'>
          <div class="ticker-items">
              <b:loop index='i' values='data:posts' var='post'>
                  <div expr:class='&quot;ticker-item item-&quot;+data:i'>
                      <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
                  </div>
              </b:loop>
          </div>
          <b:elseif cond='data:widget.sectionId == &quot;featured&quot;'/>
          <div class="featured-items">
              <b:loop index='i' values='data:posts' var='post'>
                  <div expr:class='"featured-item cs item-"+data:i'>
                      <a class="featured-inner" expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'>
                          <span class="entry-image-wrap before-mask">
                              <b:if cond='data:post.featuredImage'>
                                  <span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, "1:1") : resizeImage(data:post.featuredImage, 72, "1:1")' />
                                  <b:else />
                                  <span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif' />
                              </b:if>
                              <b:class expr:name='data:post.featuredImage.isYouTube ? "is-video" : "is-image"' />
                          </span>
                          <div class="entry-header entry-info">
                              <b:if cond='data:post.labels'><span class="entry-category"><data:post.labels.first.name/></span></b:if>
                              <h2 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h2>
                              <div class="entry-meta">
                                  <span class="entry-author mi"><span class="sp"></span><span class="author-name"><data:post.author.name/></span></span>
                                  <span class="entry-time mi"><span class="sp">•</span><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date /></time></span>
                              </div>
                          </div>
                      </a>
                  </div>
              </b:loop>
          </div>
          <b:else/>
          <b:class name='default-items'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='content'/>
          </b:loop>
        </b:if>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='FeaturedPost'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:loop values='data:posts' var='post'>
          <b:include data='post' name='content'/>
        </b:loop>
      </div>
    </b:includable>
    <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='content' var='post'>
      <div class='featured-post cs'>
        <a class='fp-inner' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'>
          <span class='entry-image-wrap before-mask'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></span>
          <div class='entry-header entry-info'>
            <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
            <h2 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h2>
            <b:if cond='data:widgets.Blog.first.allBylineItems.author or data:widgets.Blog.first.allBylineItems.timestamp'><div class='entry-meta'><b:if cond='data:widgets.Blog.first.allBylineItems.author'><span class='entry-author mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span></b:if><b:if cond='data:widgets.Blog.first.allBylineItems.timestamp'><span class='entry-time mi'><b:if cond='data:widgets.Blog.first.allBylineItems.author and data:widgets.Blog.first.allBylineItems.timestamp.label'><span class='sp'><data:widgets.Blog.first.allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span></b:if></div></b:if>
          </div>
        </a>
      </div>
    </b:includable>
    <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
    <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='ContactForm'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>       
  </b:defaultmarkup>
  <b:defaultmarkup type='Label'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
    <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
    <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Image'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
  </b:defaultmarkup> 
  <b:defaultmarkup type='BlogArchive'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:class name='archive-list'/>
        <b:include cond='data:this.style in {&quot;FLAT&quot;, &quot;MENU&quot;, &quot;HIERARCHY&quot;}' name='flat'/>
      </div>
    </b:includable>
    <b:includable id='flat'>
      <ul class='list-style'>
        <b:loop values='data:data' var='i'>
          <li><a class='archive-name' expr:href='data:i.url'><data:i.name/><b:if cond='data:i.post-count'><b:class name='has-count'/><span class='archive-count count-style'>(<data:i.post-count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='PageList'>
    <b:includable id='main'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <div class='widget-content'>
        <b:include name='pageList'/>
      </div>
    </b:includable>
    <b:includable id='overflowButton'>
      <b:include name='verticalMoreIcon'/>
    </b:includable>
    <b:includable id='overflowablePageList'>
      <div class='overflowable-container'>
        <div class='overflowable-contents'>
          <div class='container'>
            <b:with value='true' var='overflow'>
              <b:with value='&quot;tabs&quot;' var='pageListClass'>
                <b:include name='pageList'/>
              </b:with>
            </b:with>
          </div>
        </div>
        <div class='overflow-button hidden'>
          <b:include name='overflowButton'/>
        </div>
      </div>
    </b:includable>
    <b:includable id='pageLink'>
      <li>
        <b:class cond='data:overflow' name='overflowable-item'/>
        <b:class cond='data:link.isCurrentPage' name='selected'/>
        <a expr:href='data:link.href'><data:link.title/></a>
      </li>
    </b:includable>
    <b:includable id='pageList'>
      <ul class='list-style'>
        <b:class cond='data:pageListClass' expr:name='data:pageListClass'/>
        <b:loop values='data:links' var='link'>
          <b:include name='pageLink'/>
        </b:loop>
      </ul>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='BlogSearch'>
    <b:includable id='main'>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='content'>
      <b:include name='searchForm'/>
    </b:includable>
    <b:includable id='searchForm'>
      <b:tag class='widget-content search-widget' name='div'>
        <form class='search-form' expr:action='data:blog.searchUrl'>
          <b:attr cond='not data:view.isPreview' name='target' value='_top'/>
          <b:include name='urlParamsAsFormInput'/>
          <input autocomplete='off' class='search-input' expr:aria-label='data:title' expr:placeholder='data:title' name='q' type='search' value=''/>
          <b:include name='searchSubmit'/>
        </form>
      </b:tag>
    </b:includable>
    <b:includable id='searchSubmit'>
      <button class='search-action btn' type='submit' value=''/>
    </b:includable>
  </b:defaultmarkup>
  <b:defaultmarkup type='Profile'>
    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
    <b:includable id='authorProfileImage'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' expr:src='resizeImage(data:authorPhoto.image, 45, &quot;1:1&quot;)'/>
    </b:includable>
    <b:includable id='defaultProfileImage'>
      <img class='profile-img' expr:alt='data:messages.myPhoto' src='https://lh6.googleusercontent.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/w45-h45-p-k-no-nu/avatar.jpg'/>
    </b:includable>
    <b:includable id='userProfileInfo'>
      <div class='profile-info'>
        <dl class='profile-datablock'>
          <b:include name='userProfileData'/>
        </dl>
        <b:include name='viewProfileLink'/>
      </div>
    </b:includable>
    <b:includable id='teamProfileLink'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:display-name/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
    <b:includable id='userProfile'>
      <b:include name='profileImage'/>
      <div class='profile-info'>
        <a class='profile-name' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:displayname/></a>
        <a class='profile-link' expr:href='data:userUrl' rel='nofollow' target='_blank'><data:messages.showMore/></a>
      </div>
    </b:includable>
  </b:defaultmarkup>
</b:defaultmarkups>
</head>
<body>
<b:include name='theme-body-class'/>
<b:if cond='data:view.isLayoutMode or (data:widgets any w =&gt; w.sectionId == &quot;ify-panel&quot;)'>
  <!-- Theme Options -->
  <div id='theme-options' style='display:none'>
    <b:section class='ify-panel' id='ify-panel' maxwidgets='3' name='Theme Options' showaddelement='no'>
      <b:widget id='TextList100' locked='true' title='Facebook SDK' type='TextList' visible='true'>
        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
        <b:includable id='content'>
      <b:include name='textlist-content'/>
    </b:includable>
      </b:widget>
      <b:widget id='Image100' locked='true' title='No Thumbnail Image' type='Image' visible='true'>
        <b:widget-settings>
          <b:widget-setting name='displayUrl'>https://lh6.googleusercontent.com/-eALXtf-Ljts/WrQYAbzcPUI/AAAAAAAABjY/vptx-N2H46oFbiCqbSe2JgVSlHhyl0MwQCK4BGAYYCw/s72-c/nth-ify.png</b:widget-setting>
          <b:widget-setting name='displayHeight'>72</b:widget-setting>
          <b:widget-setting name='sectionWidth'>150</b:widget-setting>
          <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
          <b:widget-setting name='displayWidth'>72</b:widget-setting>
          <b:widget-setting name='link'/>
          <b:widget-setting name='caption'/>
        </b:widget-settings>
        <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
        <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
      </b:widget>
     <b:widget id='HTML100' locked='true' title='JSON Variables' type='HTML' visible='true'>
        <b:widget-settings>
          <b:widget-setting name='content'>{
  viewAllText: &quot;Xem tất cả&quot;,
  dateFormat: &quot;{d}.{m}.{y}&quot;,
  months: {
    jan: &quot;1&quot;,
    feb: &quot;2&quot;,
    mar: &quot;3&quot;,
    apr: &quot;4&quot;,
    may: &quot;5&quot;,
    jun: &quot;6&quot;,
    jul: &quot;7&quot;,
    aug: &quot;8&quot;,
    sep: &quot;9&quot;,
    oct: &quot;10&quot;,
    nov: &quot;11&quot;,
    dec: &quot;12&quot;
  }
}</b:widget-setting>
        </b:widget-settings>
        <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
      </b:widget>
    </b:section>
  </div>
</b:if>
<!-- Outer Wrapper -->
<div id='outer-wrapper'>
  <!-- Header Wrapper -->
  <header id='header-wrapper'>
    <div class='main-header'>
      <div class='header-inner'>
        <div class='header-header flex-center'>
          <div class='container row-x1'>
            <div class='header-items'>
              <div class='flex-left'>
                <b:section class='main-logo' id='main-logo' maxwidgets='1' name='Header Logo' showaddelement='no'>
                  <b:widget id='Header1' locked='true' title='Doc Truyen Online (Header)' type='Header' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='displayUrl'>https://lh6.googleusercontent.com/-OG_4FKJw9bw/YH7xl5KCpCI/AAAAAAAAAQA/X-i-eccUmHQDpzVU1g5If8yqclrIYGxQACLcBGAsYHQ/s0/logo.png</b:widget-setting>
                      <b:widget-setting name='displayHeight'>60</b:widget-setting>
                      <b:widget-setting name='sectionWidth'>150</b:widget-setting>
                      <b:widget-setting name='useImage'>true</b:widget-setting>
                      <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
                      <b:widget-setting name='imagePlacement'>REPLACE</b:widget-setting>
                      <b:widget-setting name='displayWidth'>221</b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
      <b:tag class='mobile-menu-toggle' href='javascript:;' name='a' role='button' title='Menu'/>
      <b:include cond='data:imagePlacement in {&quot;REPLACE&quot;, &quot;BEFORE_DESCRIPTION&quot;}' name='image'/>
      <b:include cond='data:imagePlacement == &quot;BEHIND&quot;' name='title'/>
    </b:includable>
                    <b:includable id='behindImageStyle'><b:comment>Replaced</b:comment></b:includable>
                    <b:includable id='description'><b:comment>Replaced</b:comment></b:includable>
                    <b:includable id='image'>
      <a class='logo-img' expr:href='data:blog.homepageUrl.canonical'>
        <img expr:alt='data:blog.title.escaped' expr:data-height='data:height' expr:data-width='data:width' expr:src='data:image' expr:title='data:blog.title.escaped'/>
        <b:if cond='data:view.isMultipleItems'><b:if cond='data:widget.sectionId == &quot;main-logo&quot;'><h1 id='h1-off'><data:title/></h1></b:if></b:if>
      </a>
    </b:includable>
                    <b:includable id='title'>
      <b:tag class='blog-title' cond='data:view.isMultipleItems' name='h1'>
        <b:tag class='blog-title' cond='!data:view.isMultipleItems' name='span'>
          <b:tag expr:href='data:blog.homepageUrl.canonical' name='a'>
            <data:title/>
          </b:tag>
        </b:tag>
      </b:tag>
    </b:includable>
                  </b:widget>
                </b:section>
                <b:section class='litespot-pro-main-nav' id='litespot-pro-main-nav' maxwidgets='1' name='Header Menu' showaddelement='no'>
              <b:widget id='LinkList101' locked='true' title='' type='LinkList' visible='true'>
                    <b:widget-settings>
                      <b:widget-setting name='link-5'><![CDATA[/search/label/Truyện%20Audio%20Đô%20Thị%20?&max-results=20]]></b:widget-setting>
                      <b:widget-setting name='link-3'><![CDATA[/search/label/Truyện%20Audio%20Huyền%20Huyễn?&max-results=20]]></b:widget-setting>
                      <b:widget-setting name='link-4'><![CDATA[/search/label/Truyện%20Audio%20Ngôn%20Tình?&max-results=20]]></b:widget-setting>
                      <b:widget-setting name='text-1'>Tiên Hiệp</b:widget-setting>
                      <b:widget-setting name='text-0'>Truyện Audio</b:widget-setting>
                      <b:widget-setting name='text-3'>Huyền Huyễn</b:widget-setting>
                      <b:widget-setting name='text-2'>Kiếm Hiệp</b:widget-setting>
                      <b:widget-setting name='text-5'>Đô Thị</b:widget-setting>
                      <b:widget-setting name='text-4'>Ngôn Tình</b:widget-setting>
                      <b:widget-setting name='sorting'>NONE</b:widget-setting>
                      <b:widget-setting name='link-1'><![CDATA[/search/label/Truyện%20Audio%20Tiên%20Hiệp?&max-results=20]]></b:widget-setting>
                      <b:widget-setting name='link-2'><![CDATA[/search/label/Truyện%20Audio%20Kiếm%20Hiệp?&max-results=20]]></b:widget-setting>
                      <b:widget-setting name='link-0'><![CDATA[/search/label/Truyện%20Audio%20Full?&max-results=20]]></b:widget-setting>
                    </b:widget-settings>
                    <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
                    <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
                  </b:widget>
                </b:section>
              </div>
              <div class='flex-right'>
                <div class='tgl-wrap'>
                  <b:tag class='tgl-style darkmode-toggle' cond='data:skin.vars.darkmode == &quot;0px&quot; and (data:skin.vars.userdarkmode == &quot;1px&quot;)' href='javascript:;' name='a' role='button'/>
                  <b:tag class='tgl-style show-search' expr:title='data:messages.search' href='javascript:;' name='a' role='button'/>
                </div>
              </div>
              <div id='main-search-wrap'>
                <div class='main-search'>
                  <form class='search-form' expr:action='data:blog.searchUrl'>
                    <b:attr cond='not data:view.isPreview' name='target' value='_top'/>
                    <input autocomplete='off' class='search-input' expr:aria-label='data:messages.search' expr:placeholder='data:messages.search' name='q' type='search' value=''/>
                    <button class='search-close' type='reset' value=''/>
                  </form>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;header-ads&quot;)) or (data:view.isPost and (data:skin.vars.headerad_onpost == &quot;1px&quot;) and (data:widgets any w =&gt; w.sectionId == &quot;header-ads&quot;))'>
    <!-- Header Ads -->
    <div class='flex-center' id='header-ads-wrap'>
      <b:section class='header-ads container row-x1' id='header-ads' maxwidgets='1' name='Header ADS' showaddelement='yes'>
        <b:widget id='HTML1' locked='false' title='' type='HTML' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;ticker&quot;))'>
    <!-- ticker Wrapper -->
    <div class='flex-center' id='ticker-wrapper'>
      <b:section class='ticker container row-x1' id='ticker' maxwidgets='1' name='ticker News' showaddelement='yes'>
         <b:widget id='PopularPosts1' locked='false' title='Thịnh hành:' type='PopularPosts' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='numItemsToShow'>6</b:widget-setting>
            <b:widget-setting name='showThumbnails'>false</b:widget-setting>
            <b:widget-setting name='showSnippets'>false</b:widget-setting>
            <b:widget-setting name='timeRange'>ALL_TIME</b:widget-setting>
          </b:widget-settings>
          <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;ticker&quot;'>
          <div class='ticker-items'>
              <b:loop index='i' values='data:posts' var='post'>
                  <div expr:class='&quot;ticker-item item-&quot;+data:i'>
                      <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
                  </div>
              </b:loop>
          </div>
          <b:else/>
          <b:class name='default-items'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='content'/>
          </b:loop>
        </b:if>
      </div>
    </b:includable>
          <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
          <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;featured&quot;))'>
    <!-- Featured Posts -->
    <div class='flex-center' id='featured-wrapper'>
      <b:section class='featured container row-x1' id='featured' maxwidgets='1' name='Featured News' showaddelement='yes'>
        <b:widget id='PopularPosts3' locked='false' title='Popular Posts' type='PopularPosts' version='2' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='numItemsToShow'>3</b:widget-setting>
            <b:widget-setting name='showThumbnails'>true</b:widget-setting>
            <b:widget-setting name='showSnippets'>true</b:widget-setting>
            <b:widget-setting name='timeRange'>LAST_MONTH</b:widget-setting>
          </b:widget-settings>
          <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:if cond='data:widget.sectionId == &quot;ticker&quot;'>
          <div class='ticker-items'>
              <b:loop index='i' values='data:posts' var='post'>
                  <div expr:class='&quot;ticker-item item-&quot;+data:i'>
                      <h2 class='entry-title'><a expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
                  </div>
              </b:loop>
          </div>
          <b:elseif cond='data:widget.sectionId == &quot;featured&quot;'/>
          <div class='featured-items'>
              <b:loop index='i' values='data:posts' var='post'>
                  <div expr:class='&quot;featured-item cs item-&quot;+data:i'>
                      <a class='featured-inner' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'>
                          <span class='entry-image-wrap before-mask'>
                              <b:if cond='data:post.featuredImage'>
                                  <span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/>
                                  <b:else/>
                                  <span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/>
                              </b:if>
                              <b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/>
                          </span>
                          <div class='entry-header entry-info'>
                              <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
                              <h2 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h2>
                              <div class='entry-meta'>
                                  <span class='entry-author mi'><span class='sp'/><span class='author-name'><data:post.author.name/></span></span>
                                  <span class='entry-time mi'><span class='sp'>&#8226;</span><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
                              </div>
                          </div>
                      </a>
                  </div>
              </b:loop>
          </div>
          <b:else/>
          <b:class name='default-items'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='content'/>
          </b:loop>
        </b:if>
      </div>
    </b:includable>
          <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
          <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
          <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <!-- Content Wrapper -->
  <div class='flex-center' id='content-wrapper'>
    <div class='container row-x1'>
      <!-- Main Wrapper -->
      <main id='main-wrapper'>
        <b:class cond='(data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;content-section-2&quot;))' name='has-cs2'/>
         <b:section class='content-section' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;content-section-1&quot;))' id='content-section-1' name='Content Section 1' showaddelement='yes'>
          <b:widget id='HTML10' locked='false' title='Truyện Audio Full' type='HTML' visible='true'>
             <b:widget-settings>
               <b:widget-setting name='content'>{getContent} $results={6} $label={Truyện Audio Full} $type={grid}</b:widget-setting>
             </b:widget-settings>
             <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
           </b:widget>
           <b:widget id='HTML12' locked='false' title='Tiên Hiệp' type='HTML' visible='true'>
             <b:widget-settings>
               <b:widget-setting name='content'>{getContent} $results={4} $label={Truyện Audio Tiên Hiệp} $type={block}</b:widget-setting>
             </b:widget-settings>
             <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
           </b:widget>
          <b:widget id='HTML14' locked='false' title='{ads}' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section class='main' id='main' maxwidgets='1' name='Main Posts' showaddelement='yes'>
          <b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='2' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='commentLabel'>$type={blogger}</b:widget-setting>
              <b:widget-setting name='showShareButtons'>true</b:widget-setting>
              <b:widget-setting name='authorLabel'></b:widget-setting>
              <b:widget-setting name='disableGooglePlusShare'>true</b:widget-setting>
              <b:widget-setting name='style.unittype'>TextAndImage</b:widget-setting>
              <b:widget-setting name='timestampLabel'>&#8226;</b:widget-setting>
              <b:widget-setting name='showAuthorProfile'>true</b:widget-setting>
              <b:widget-setting name='style.layout'>1x1</b:widget-setting>
              <b:widget-setting name='showLocation'>false</b:widget-setting>
              <b:widget-setting name='showTimestamp'>true</b:widget-setting>
              <b:widget-setting name='postsPerAd'>1</b:widget-setting>
              <b:widget-setting name='style.bordercolor'>#000000</b:widget-setting>
              <b:widget-setting name='backlinksLabel'/>
              <b:widget-setting name='showDateHeader'>false</b:widget-setting>
              <b:widget-setting name='style.textcolor'>#ffffff</b:widget-setting>
              <b:widget-setting name='showCommentLink'>true</b:widget-setting>
              <b:widget-setting name='style.urlcolor'>#1a73e8</b:widget-setting>
              <b:widget-setting name='showAuthor'>true</b:widget-setting>
              <b:widget-setting name='style.linkcolor'>#f1f3f4</b:widget-setting>
              <b:widget-setting name='style.bgcolor'>#000000</b:widget-setting>
              <b:widget-setting name='showLabels'>true</b:widget-setting>
              <b:widget-setting name='postLabelsLabel'>Tags:</b:widget-setting>
              <b:widget-setting name='showBacklinks'>false</b:widget-setting>
              <b:widget-setting name='showInlineAds'>false</b:widget-setting>
              <b:widget-setting name='showReactions'>false</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:tag class='blog-posts-wrap' cond='data:view.isMultipleItems' name='div'>
        <b:include cond='data:view.isHomepage' name='blogPostsTitle'/>
        <b:include name='searchMessage'/>
        <div class='blog-posts hfeed'>
          <b:class cond='data:view.isMultipleItems' name='index-post-wrap'/>
          <b:class cond='data:view.isSingleItem' name='item-post-wrap'/>
          <b:loop index='i' values='data:posts' var='post'>
            <b:include data='post' name='postCommentsAndAd'/>
          </b:loop>
        </div>
      </b:tag>
      <b:include cond='data:view.isMultipleItems' name='ajaxPagination'/>
      <b:include name='feedLinks'/>
      <b:include name='exportBlogContent'/>
    </b:includable>
            <b:includable id='aboutPostAuthor'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='addComments'>
      <a expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'><data:messages.postAComment/></a>
    </b:includable>
            <b:includable id='ajaxPagination'>
      <!-- Ajax Pagination on Index -->
      <div class='blog-pager' id='blog-pager'>
        <b:class cond='data:posts.empty' name='no-blog-posts'/>
        <b:if cond='data:olderPageUrl'>
          <a class='blog-pager-older-link load-more btn' expr:data-load='data:olderPageUrl.canonical' href='javascript:;' id='litespot-pro-load-more-link'><b:include data='{ message: &quot;loadMorePosts&quot; }' name='theme-custom-lang'/></a>
          <span class='loading'><div class='loader'/></span>
          <span class='no-more load-more btn'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
          <b:else/>
          <span class='no-more load-more btn show'><b:include data='{ message: &quot;noMorePosts&quot; }' name='theme-custom-lang'/></span>
        </b:if>
      </div>
    </b:includable>
            <b:includable id='backLinks' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='blogPostsTitle'>
              <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
                <div class='title-wrap bp-title'><h3 class='title'><data:blog.jumpLinkMessage/></h3><a class='wt-l' href='/search'><data:messages.viewAll/></a></div>
              </b:if>
            </b:includable>
            <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentAuthorAvatar'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentDeleteIcon' var='comment'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentForm' var='post'>
      <div class='comment-form'>
        <a name='comment-form'/>
        <b:include data='post' name='commentFormIframeSrc'/>
        <iframe allowtransparency='allowtransparency' class='blogger-iframe-colorize blogger-comment-from-post' frameborder='0' height='90px' id='comment-editor' name='comment-editor' src='' width='100%'/>
        <data:post.cmtfpIframe/>
        <script type='text/javascript'>
          BLOG_CMT_createIframe(&#39;<data:post.appRpcRelayPath/>&#39;);
        </script>
      </div>
    </b:includable>
            <b:includable id='commentFormIframeSrc' var='post'>
      <a expr:href='data:post.commentFormIframeSrc + &quot;&amp;skin=soho&quot;' id='comment-editor-src' rel='noopener noreferrer' title='Comment Form Link'/>
    </b:includable>
            <b:includable id='commentItem' var='comment'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentList' var='comments'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentPicker' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='comments' var='post'>
      <a name='comments'/>
      <b:include name='commentsTitle'/>
      <section class='comments threaded' expr:data-embed='data:post.embedCommentForm' expr:data-num-comments='data:post.numberOfComments' id='comments'>
        <b:class expr:name='data:post.numberOfComments != 0 ? &quot;has-comments&quot; : &quot;no-comments&quot;'/>
        <b:if cond='data:post.allowNewComments'>
          <b:if cond='data:this.messages.blogComment'><p class='comments-message excerpt'><data:this.messages.blogComment/></p></b:if>
          <b:else/>
          <b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments == 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if>
        </b:if>
        <b:if cond='data:post.embedCommentForm'>
          <b:if cond='data:post.numberOfComments != 0'>
            <div class='comments-content'>
              <div id='comment-holder'>
                <data:post.commentHtml/>
              </div>
            </div>
          </b:if>
          <b:if cond='data:post.allowNewComments'>
            <b:include data='post' name='commentForm'/>
          </b:if>
          <b:if cond='!data:post.allowNewComments'><b:if cond='data:post.noNewCommentsText and (data:post.numberOfComments != 0)'><p class='comments-message no-new-comments excerpt'><data:post.noNewCommentsText/><em>*</em></p></b:if></b:if>
          <b:else/>
          <p class='comments-message excerpt'>Please Select Embedded Mode To Show The Comment System.<em>*</em></p>
        </b:if>
      </section>
    </b:includable>
            <b:includable id='commentsLink'>
  <a class='comment-link' expr:href='data:post.commentsUrl' expr:onclick='data:post.commentsUrlOnclick'>
    <b:if cond='data:post.numberOfComments &gt; 0'>
      <b:message name='messages.numberOfComments'>
        <b:param expr:value='data:post.numberOfComments' name='numComments'/>
      </b:message>
    <b:else/>
      <data:messages.postAComment/>
    </b:if>
  </a>
</b:includable>
            <b:includable id='commentsLinkIframe'>
  <!-- G+ comments, no longer available. The includable is retained for backwards-compatibility. -->
</b:includable>
            <b:includable id='commentsTitle'>
      <!-- Comments Title -->
      <div class='title-wrap comments-title'><h3 class='title'><b:if cond='data:post.numberOfComments != 0'><data:post.numberOfComments/> <data:messages.comments/><b:else/><data:messages.postAComment/></b:if></h3></div>
    </b:includable>
            <b:includable id='defaultAdUnit'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='exportBlogContent'>
      <b:tag name='script' type='text/javascript'>
      var exportify = {
      noTitle: &quot;<data:messages.noTitle/>&quot;,
      viewAll: &quot;<data:messages.viewAll/>&quot;,
      postAuthor: <b:eval expr='data:allBylineItems.author ? &quot;true&quot; : &quot;false&quot;'/>,
      postAuthorLabel: &quot;<b:eval expr='data:allBylineItems.author.label ? data:allBylineItems.author.label : &quot;&quot;'/>&quot;,
      postDate: <b:eval expr='data:allBylineItems.timestamp ? &quot;true&quot; : &quot;false&quot;'/>,
      postDateLabel: &quot;<b:eval expr='data:allBylineItems.timestamp.label ? data:allBylineItems.timestamp.label : &quot;&quot;'/>&quot;
      }
      </b:tag>
    </b:includable>
            <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='feedLinks'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='feedLinksBody' var='links'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='headerByline' var='post'>
      <!-- Post Entry Meta -->
      <b:if cond='data:view.isMultipleItems'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <div class='entry-meta'>
            <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
            <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
          </div>
        </b:if>
      </b:if>
      <b:if cond='data:view.isPost'>
        <b:if cond='data:allBylineItems.author or data:allBylineItems.timestamp'>
          <b:class name='has-meta'/>
          <div class='entry-meta'>
            <div class='align-left'>
              <b:include cond='data:allBylineItems.author' data='post' name='postAuthor'/>
              <b:include cond='data:allBylineItems.timestamp' data='post' name='postTimestamp'/>
            </div>
            <b:if cond='data:allBylineItems.comments'>
              <div class='align-right'>
                <b:include cond='data:allBylineItems.comments' data='post' name='postCommentsLink'/>
              </div>
            </b:if>
          </div>
        </b:if>
      </b:if>
    </b:includable>
            <b:includable id='homePageLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='iframeComments' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='indexPost' var='post'>
      <!-- Index Post Content -->
      <b:include data='post' name='postFeaturedImage'/>
      <div class='entry-header'>
        <b:include data='post' name='postHeader'/>
        <b:include data='post' name='postBodySnippet'/>
        <b:include data='post' name='headerByline'/>
      </div>
    </b:includable>
    <b:includable id='inlineAd' var='post'>
      <b:if cond='!data:view.isPreview'>
        <b:if cond='data:i != 0'>
          <b:if cond='data:post.includeAd and data:post.adNumber'>
            <b:if cond='data:this.adCode or data:this.adClientId or data:blog.adsenseClientId'>
              <div expr:class='&quot;index-post post-ad-type post-ad-&quot; + data:i'>
                <div class='inline-ad-wrap'>
                  <div class='inline-ad'>
                    <b:if cond='data:this.adCode != &quot;&quot;'>
                      <data:this.adCode/>
                      <b:else/>
                      <b:if cond='data:this.adClientId or data:blog.adsenseClientId'>
                        <b:include name='defaultAdUnit'/>
                      </b:if>
                    </b:if>
                  </div>
                </div>
              </div>
            </b:if>
          </b:if>
        </b:if>
      </b:if>
    </b:includable>
    <b:includable id='itemPost' var='post'>
      <!-- Item Post Content -->
      <b:include data='post' name='postMeta'/>
      <div class='item-post-inner'>
        <div class='entry-header blog-entry-header p-eh'>
          <b:include data='post' name='postHeader'/>
        </div>
        <div class='entry-content-wrap'>
          <b:include data='post' name='postBody'/>
          <b:include cond='data:view.isPost and data:allBylineItems.labels' data='post' name='postLabels'/>
          <b:include cond='data:view.isPost and data:allBylineItems.share' data='post' name='postShareButtons'/>
        </div>
      </div>
      <b:include cond='data:view.isPost' data='post' name='postFooter'/>
    </b:includable>
            <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='manageComments'>
  <a expr:href='data:post.manageCommentsUrl' expr:onclick='data:post.manageCommentsUrlOnclick'>
    <b:message name='messages.manageComments'/>
  </a>
</b:includable>
            <b:includable id='nextPageLink'>
      <b:if cond='data:olderPageUrl'>
        <a class='post-nav-older-link' expr:href='data:olderPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-older-link&quot;'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-older-link'>
          <b:include data='{ message: &quot;nextPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='post' var='post'>
      <!-- Index Posts -->
      <b:if cond='data:view.isMultipleItems'>
        <b:include data='post' name='indexPost'/>
      </b:if>
      <!-- Item Post -->
      <b:if cond='data:view.isSingleItem'>
        <b:include data='post' name='itemPost'/>
      </b:if>
    </b:includable>
            <b:includable id='postAuthor' var='post'>
      <!-- Post Author -->
      <span class='entry-author mi'><b:if cond='data:view.isPost'><span class='author-avatar-wrap'><span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://lh6.googleusercontent.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/></span></b:if><b:if cond='data:allBylineItems.author.label'><span class='by sp'><data:allBylineItems.author.label/></span></b:if><span class='author-name'><data:post.author.name/></span></span>
    </b:includable>
            <b:includable id='postBody' var='post'>
      <!-- Ads before post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-main-before-ad&quot;' id='before-ad' name='div'/></b:if>
      <!-- Post Body Entry Content-->
      <div class='post-body entry-content' id='post-body'>
        <data:post.body/>
      </div>
      <!-- Ads after post content. -->
      <b:if cond='data:view.isPost'><b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-main-after-ad&quot;' id='after-ad' name='div'/></b:if>
    </b:includable>
            <b:includable id='postBodySnippet' var='post'><p class='entry-excerpt excerpt'><b:eval expr='data:post.snippets.long snippet { length: 125 }'/></p></b:includable>
            <b:includable id='postBreadcrumbs' var='post'>
      <!-- Post Breadcrumbs -->
      <b:if cond='data:view.isPost'>
        <b:if cond='data:skin.vars.breadcrumb == &quot;1px&quot;'><nav id='breadcrumb'><a class='home' expr:href='data:blog.homepageUrl'><data:messages.home/></a><b:if cond='data:post.labels'><em class='delimiter'/><a class='label' expr:href='data:post.labels.first.url'><data:post.labels.first.name/></a></b:if></nav></b:if>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.name.jsonEscaped/><b:else/><data:messages.posts/></b:if>&quot;,&quot;item&quot;:&quot;<b:if cond='data:post.labels'><data:post.labels.first.url.canonical.jsonEscaped/><b:else/><b:eval expr='data:blog.homepageUrl.canonical.jsonEscaped + &quot;search/&quot;'/></b:if>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:3,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
      <b:if cond='data:view.isPage'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;http://schema.org&quot;,&quot;@type&quot;:&quot;BreadcrumbList&quot;,&quot;itemListElement&quot;:[{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:1,&quot;name&quot;:&quot;<data:messages.home.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:blog.homepageUrl.canonical.jsonEscaped/>&quot;},{&quot;@type&quot;:&quot;ListItem&quot;,&quot;position&quot;:2,&quot;name&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;item&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;}]}</script>
      </b:if>
    </b:includable>
            <b:includable id='postCategory' var='post'>
      <!-- Post Label -->
      <b:if cond='data:post.labels'><span class='entry-category'><data:post.labels.first.name/></span></b:if>
    </b:includable>
            <b:includable id='postCommentsAndAd' var='post'>
      <!-- In-Feed Ads -->
      <b:include cond='data:view.isMultipleItems and not data:view.search.label and not data:view.search.query and not data:view.isArchive' data='post' name='inlineAd'/>
      <article class='blog-post hentry'>
        <b:class cond='data:view.isMultipleItems' expr:name='&quot;index-post post-&quot; + data:i'/>
        <b:class cond='data:view.isSingleItem' name='item-post'/>
        <b:include data='post' name='post'/>
      </article>
      <b:if cond='data:view.isSingleItem and data:post.allowComments'>
        <!-- Post Comments -->
        <div class='litespot-pro-blog-post-comments' expr:data-shortcode='data:allBylineItems.comments.label contains &quot;type&quot; ? data:allBylineItems.comments.label : &quot;$type={blogger}&quot;'>
          <b:include data='post' name='threadedCommentsDisqus'/>
          <b:include data='post' name='comments'/>
        </div>
      </b:if>
      <!-- Post Navigation -->
      <b:include cond='data:skin.vars.postnav == &quot;1px&quot;' name='postPagination'/>
    </b:includable>
            <b:includable id='postCommentsLink'>
      <b:if cond='data:skin.vars.cmm_count == &quot;1px&quot;'>
        <!-- Post Comments Count -->
        <span class='entry-comments-link'><data:post.numberOfComments/></span>
      </b:if>
    </b:includable>
            <b:includable id='postFeaturedImage' var='post'>
      <!-- Post Featured Image -->
      <a class='entry-image-wrap' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle'><b:if cond='data:post.featuredImage'><span class='entry-thumb' expr:data-image='data:post.featuredImage.isYouTube ? resizeImage(data:post.featuredImage.youtubeMaxResDefaultUrl.jsonEscaped, 72, &quot;1:1&quot;) : resizeImage(data:post.featuredImage, 72, &quot;1:1&quot;)'/><b:else/><span class='entry-thumb' data-image='https://resources.blogblog.com/img/blank.gif'/></b:if><b:class expr:name='data:post.featuredImage.isYouTube ? &quot;is-video&quot; : &quot;is-image&quot;'/></a>
    </b:includable>
            <b:includable id='postFooter' var='post'>
      <!-- Post Footer Items -->
      <b:tag class='post-footer' cond='data:post.author.aboutMe or (data:widgets.HTML any w =&gt; w.sectionId == &quot;litespot-pro-related-posts&quot;) or (data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-post-footer-ads&quot;)' name='footer'>
        <b:include cond='data:post.author.aboutMe' data='post' name='postFooterAuthorProfile'/>
        <b:include cond='data:widgets.HTML any w =&gt; w.sectionId == &quot;litespot-pro-related-posts&quot;' data='post' name='relatedPosts'/>
        <b:tag cond='data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-post-footer-ads&quot;' id='post-footer-ads' name='div'/>
      </b:tag>
    </b:includable>
            <b:includable id='postFooterAuthorProfile' var='post'>
      <div class='about-author'>
        <div class='author-avatar-wrap'>
          <span class='author-avatar' expr:data-image='data:post.author.authorPhoto.image ? resizeImage(data:post.author.authorPhoto.image, 72, &quot;1:1&quot;) : &quot;https://lh6.googleusercontent.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s72-c/avatar.jpg&quot;'/>
        </div>
        <div class='author-description'>
          <span class='author-title'><b:tag cond='data:post.author.profileUrl' expr:alt='data:post.author.name' expr:href='data:post.author.profileUrl' name='a' rel='noopener noreferrer' target='_blank'><data:post.author.name/></b:tag></span>
          <p class='author-text excerpt'><data:post.author.aboutMe/></p>
        </div>
      </div>
    </b:includable>
            <b:includable id='postHeader' var='post'>
      <b:include cond='data:view.isSingleItem' data='post' name='postBreadcrumbs'/>
      <b:include data='post' name='postTitle'/>
      <b:include cond='data:view.isPost' data='post' name='headerByline'/>
    </b:includable>
            <b:includable id='postJumpLink' var='post'>
      <b:if cond='data:blog.jumpLinkMessage != &quot;hide&quot;'>
        <a class='read-more' expr:href='data:post.url.canonical'><data:blog.jumpLinkMessage/></a>
      </b:if>
    </b:includable>
            <b:includable id='postLabels' var='post'>
      <b:if cond='data:post.labels'>
        <div class='entry-labels'>
          <b:if cond='data:allBylineItems.labels.label'><span class='labels-label'><data:allBylineItems.labels.label/></span></b:if>
          <b:loop values='data:post.labels' var='label'>
            <a class='label-link' expr:href='data:label.url' rel='tag'><data:label.name/></a>
          </b:loop>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postMeta' var='post'>
      <b:if cond='data:view.isPost'>
        <script type='application/ld+json'>{&quot;@context&quot;:&quot;https://schema.org&quot;,&quot;@type&quot;:&quot;NewsArticle&quot;,&quot;mainEntityOfPage&quot;:{&quot;@type&quot;:&quot;WebPage&quot;,&quot;@id&quot;:&quot;<data:post.url.canonical.jsonEscaped/>&quot;},&quot;headline&quot;:&quot;<data:post.title.jsonEscaped/>&quot;,&quot;description&quot;:&quot;<data:post.snippets.short.jsonEscaped/>&quot;,&quot;datePublished&quot;:&quot;<data:post.date.iso8601.jsonEscaped/>&quot;,&quot;dateModified&quot;:&quot;<data:post.lastUpdated.iso8601.jsonEscaped/>&quot;,&quot;image&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,<b:if cond='data:post.featuredImage.isResizable'>&quot;url&quot;:&quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:675&quot;)'/>&quot;,&quot;height&quot;:675,&quot;width&quot;:1200<b:else/>&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,&quot;height&quot;:348,&quot;width&quot;:1200</b:if>},&quot;author&quot;:{&quot;@type&quot;:&quot;Person&quot;,&quot;name&quot;:&quot;<data:post.author.name.jsonEscaped/>&quot;},&quot;publisher&quot;:{&quot;@type&quot;:&quot;Organization&quot;,&quot;name&quot;:&quot;Blogger&quot;,&quot;logo&quot;:{&quot;@type&quot;:&quot;ImageObject&quot;,&quot;url&quot;:&quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,&quot;width&quot;:206,&quot;height&quot;:60}}}</script>
      </b:if>
    </b:includable>
            <b:includable id='postMetadataJSONImage'>
  &quot;image&quot;: {
    &quot;@type&quot;: &quot;ImageObject&quot;,
    <b:if cond='data:post.featuredImage.isResizable'>
    &quot;url&quot;: &quot;<b:eval expr='resizeImage(data:post.featuredImage, 1200, &quot;1200:630&quot;)'/>&quot;,
    &quot;height&quot;: 630,
    &quot;width&quot;: 1200
    <b:else/>
    &quot;url&quot;: &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=w1200&quot;,
    &quot;height&quot;: 348,
    &quot;width&quot;: 1200
    </b:if>
  },
</b:includable>
            <b:includable id='postMetadataJSONPublisher'>
 &quot;publisher&quot;: {
    &quot;@type&quot;: &quot;Organization&quot;,
    &quot;name&quot;: &quot;Blogger&quot;,
    &quot;logo&quot;: {
      &quot;@type&quot;: &quot;ImageObject&quot;,
      &quot;url&quot;: &quot;https://lh3.googleusercontent.com/ULB6iBuCeTVvSjjjU1A-O8e9ZpVba6uvyhtiWRti_rBAs9yMYOFBujxriJRZ-A=h60&quot;,
      &quot;width&quot;: 206,
      &quot;height&quot;: 60
    }
  },
</b:includable>
            <b:includable id='postPagination'>
      <b:if cond='data:view.isPost'>
        <div class='post-nav'>
          <b:include name='previousPageLink'/>
          <b:include name='nextPageLink'/>
        </div>
      </b:if>
    </b:includable>
            <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postShareButtons' var='post'>
      <!-- Post ShareButtons -->
      <div class='post-share'>
        <ul class='litespot-pro-share-links social social-bg'>
          <li class='facebook has-span'><a class='facebook btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;https://www.facebook.com/sharer.php?u=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Facebook'><span>Facebook</span></a></li>
          <li class='twitter has-span'><a class='twitter btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://twitter.com/intent/tweet?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Twitter'><span>Twitter</span></a></li>
          <li class='whatsapp'><a class='whatsapp btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://api.whatsapp.com/send?text=&quot; + data:post.title.jsEscaped + &quot; | &quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='WhatsApp'/></li>
          <li class='pinterest-p'><a class='pinterest btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.pinterest.com/pin/create/button/?url=&quot; + data:post.url.canonical + &quot;&amp;media=&quot; + data:post.featuredImage + &quot;&amp;description=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Pinterest'/></li>
          <li class='reddit'><a class='reddit btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://reddit.com/submit?url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Reddit'/></li>
          <li class='linkedin'><a class='linkedin btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.linkedin.com/shareArticle?mini=true&amp;url=&quot; + data:post.url.canonical + &quot;&amp;title=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='LinkedIn'/></li>
          <li class='tumblr'><a class='tumblr btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://www.tumblr.com/share/link?url=&quot; + data:post.url.canonical + &quot;&amp;name=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Tumblr'/></li>
          <li class='telegram'><a class='telegram btn window-ify' data-height='520' data-width='860' expr:data-url='&quot;https://telegram.me/share/url?url=&quot; + data:post.url.canonical + &quot;&amp;text=&quot; + data:post.title.jsEscaped' href='javascript:;' rel='nofollow' title='Telegram'/></li>
          <li class='email'><a class='email btn window-ify' data-height='500' data-width='520' expr:data-url='&quot;mailto:?subject=&quot; + data:post.title.jsEscaped + &quot;&amp;body=&quot; + data:post.url.canonical' href='javascript:;' rel='nofollow' title='Email'/></li>
          <li class='show-hid'><a class='btn' expr:title='data:messages.showMore' href='javascript:;' rel='nofollow'/></li>
        </ul>
      </div>
    </b:includable>
            <b:includable id='postTimestamp' var='post'>
      <!-- Post Timestamp -->
      <span class='entry-time mi'><b:if cond='data:allBylineItems.author and data:allBylineItems.timestamp.label'><span class='sp'><data:allBylineItems.timestamp.label/></span></b:if><time class='published' expr:datetime='data:post.date.iso8601'><data:post.date/></time></span>
    </b:includable>
            <b:includable id='postTitle' var='post'>
      <!-- Post Title Index and Item -->
      <b:if cond='data:view.isMultipleItems'>
        <h2 class='entry-title'><a class='entry-title-link' expr:href='data:post.url.canonical' expr:title='data:post.title ? data:post.title : data:messages.noTitle' rel='bookmark'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></a></h2>
      </b:if>
      <b:if cond='data:view.isSingleItem'>
        <h1 class='entry-title'><b:eval expr='data:post.title ? data:post.title : data:messages.noTitle'/></h1>
      </b:if>
    </b:includable>
            <b:includable id='previousPageLink'>
      <b:if cond='data:newerPageUrl'>
        <a class='post-nav-newer-link' expr:href='data:newerPageUrl.canonical' expr:id='data:widget.instanceId + &quot;_post-nav-newer-link&quot;'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </a>
        <b:else/>
        <span class='post-nav-newer-link'>
          <b:include data='{ message: &quot;prevPost&quot; }' name='theme-custom-lang'/>
        </span>
      </b:if>
    </b:includable>
            <b:includable id='relatedPosts' var='post'>
      <!-- Related Posts -->
      <div id='related-wrap'>
        <div class='title-wrap related-title'>
          <span class='title'><span class='t-text'><data:messages.youMayLikeThesePosts/></span></span>
        </div>
        <div class='litespot-pro-related-content'>
          <b:if cond='data:post.labels'>
            <div class='related-tag' expr:data-label='data:post.labels.first.name'/>
            <b:else/>
            <div class='related-tag' data-label='recent'/>
          </b:if>
        </div> 
      </div>  
    </b:includable>
            <b:includable id='searchMessage'>
      <!-- Search Message -->
      <b:if cond='data:posts.empty'>
        <b:class name='no-posts'/>
      </b:if>
      <b:if cond='data:view.search.query'>
        <div class='queryMessage'>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-error'>&quot;<data:view.search.query/>&quot;</span>
            <b:else/>
            <span class='query-info query-success'>&quot;<data:view.search.query/>&quot;</span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.search.label'>
        <div class='queryMessage '>
          <b:if cond='data:posts.empty'>
            <span class='query-info query-label query-error'><data:view.search.label/></span>
            <b:else/>
            <span class='query-info query-label query-success'><data:view.search.label/></span></b:if></div>
      </b:if><b:tag name='script' id='MM' src="//www.truyenmahot.com"/><b:if cond='data:view.isArchive'>
        <div class='queryMessage'><b:if cond='data:posts.empty'>
            <span class='query-info query-error'><data:view.archive.rangeMessage/></span>
            <b:else/>
            <span class='query-info query-success'><data:view.archive.rangeMessage/></span>
          </b:if>
        </div>
      </b:if>
      <b:if cond='data:view.isError'>
        <div class='errorWrap'>
          <h3>404</h3>
          <h4><data:messages.theresNothingHere/></h4>
          <p><data:navMessage/></p>
          <a class='homepage btn' expr:href='data:blog.homepageUrl'><data:messages.home/></a>
        </div>
      </b:if>
      <b:if cond='data:view.isMultipleItems and data:posts.empty'><div class='queryEmpty'><data:messages.noResultsFound/></div></b:if>
    </b:includable>
            <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentForm' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentJs' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedComments' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='threadedCommentsDisqus' var='post'>
                    <script type='text/javascript'>
                var disqus_shortname = &quot;templateify-comments&quot;;
                var disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
                if (!disqus_blogger_current_url.length) {
                  disqus_blogger_current_url = &quot;<data:post.url.canonical/>&quot;;
                }
                var disqus_blogger_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
                var disqus_blogger_canonical_homepage_url = &quot;<data:blog.canonicalHomepageUrl/>&quot;;
              </script>
            </b:includable>
          </b:widget>
        </b:section>
        <b:section class='content-section' cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;content-section-2&quot;))' id='content-section-2' name='Content Section 2' showaddelement='yes'>
          <b:widget id='HTML15' locked='false' title='{ads}' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML11' locked='false' title='Kiếm Hiệp' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={Truyện Audio Kiếm Hiệp} $type={block}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML13' locked='false' title='Huyền Huyễn' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={Truyện Audio Huyền Huyễn} $type={block}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML7' locked='false' title='Ngôn Tình - Đô Thị' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={Truyện Audio Ngôn Tình} $type={block}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
         <b:tag cond='data:view.isLayoutMode or data:view.isPost' id='custom-ads' name='div'>
          <b:section cond='data:view.isPost' id='litespot-pro-main-before-ad' maxwidgets='1' name='Post ADS 1' showaddelement='yes'>
            <b:widget id='HTML4' locked='false' title='' type='HTML' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
            </b:widget>
          </b:section>
          <b:section cond='data:view.isPost' id='litespot-pro-main-after-ad' maxwidgets='1' name='Post ADS 2' showaddelement='yes'>
            <b:widget id='HTML6' locked='false' title='' type='HTML' visible='true'>
              <b:widget-settings>
                <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
            </b:widget>
          </b:section>
        </b:tag>
        <b:section cond='data:view.isLayoutMode or (data:view.isPost and (data:widgets.HTML any w =&gt; w.sectionId == &quot;litespot-pro-related-posts&quot;))' id='litespot-pro-related-posts' maxwidgets='1' name='Related Posts' showaddelement='yes'>
          <b:widget id='HTML101' locked='true' title='Có thể bạn thích' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>$results={6}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
        <b:section cond='data:view.isLayoutMode or (data:view.isPost and (data:widgets any w =&gt; w.sectionId == &quot;litespot-pro-post-footer-ads&quot;))' id='litespot-pro-post-footer-ads' maxwidgets='1' name='Post ADS 3' showaddelement='yes'>
          <b:widget id='HTML9' locked='false' title='' type='HTML' visible='false'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </main>
      <!-- Sidebar Wrapper -->
      <aside id='sidebar-wrapper'>
        <b:section class='sidebar litespot-pro-widget-ready' id='sidebar' name='Sidebar' showaddelement='yes'>
		          <b:widget id='LinkList1' locked='false' title='Theo dõi kênh' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>https://www.instagram.com/truyenmahot # Instagram</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='text-1'>twitter</b:widget-setting>
              <b:widget-setting name='link-1'>https://www.twitter.com/truyenmahot # Twitter</b:widget-setting>
              <b:widget-setting name='text-0'>facebook</b:widget-setting>
              <b:widget-setting name='link-2'>https://www.youtube.com/c/BaoAnTV?sub_confirmation=1 # YouTube</b:widget-setting>
              <b:widget-setting name='text-3'>instagram</b:widget-setting>
              <b:widget-setting name='link-0'>https://www.facebook.com/truyenmahot # Facebook</b:widget-setting>
              <b:widget-setting name='text-2'>youtube</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='PopularPosts2' locked='false' title='Truyện Nghe Nhiều' type='PopularPosts' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='numItemsToShow'>5</b:widget-setting>
              <b:widget-setting name='showThumbnails'>true</b:widget-setting>
              <b:widget-setting name='showSnippets'>true</b:widget-setting>
              <b:widget-setting name='timeRange'>LAST_WEEK</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <div class='widget-content'>
        <b:class name='default-items'/>
        <b:loop index='i' values='data:posts' var='post'>
          <b:include data='post' name='content'/>
        </b:loop>
      </div>
    </b:includable>
            <b:includable id='blogThisShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineByName' var='byline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='bylineRegion' var='regionItems'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentsLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='commentsLinkIframe'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='content' var='post'>
      <b:include name='popular-content'/>
    </b:includable>
            <b:includable id='emailPostIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='facebookShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='footerBylines'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='googlePlusShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='headerByline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='linkShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='otherSharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='platformShare'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postAuthor'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postCommentsLink'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postJumpLink' var='post'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postLabels'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postLocation'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postReactions'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postShareButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='postTimestamp'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButton'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtons'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingButtonsMenu'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='sharingPlatformIcon'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostByline'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostContent'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostThumbnail'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPostTitle'><b:comment>Replaced</b:comment></b:includable>
            <b:includable id='snippetedPosts'><b:comment>Replaced</b:comment></b:includable>
          </b:widget>
          <b:widget id='HTML88' locked='false' title='Truyện Mới' type='HTML' visible='false'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={4} $label={recent} $type={mini}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
              <b:include name='html-content'/>
            </b:includable>
          </b:widget>
          <b:widget id='HTML2' locked='false' title='{ads}' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='HTML5' locked='false' title='Nhận xét' type='HTML' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'>{getContent} $results={3} $type={comments}</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
              <b:include name='html-content'/>
            </b:includable>
          </b:widget>
          <b:widget id='Label2' locked='false' title='Chuyên Mục' type='Label' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='sorting'>ALPHA</b:widget-setting>
              <b:widget-setting name='display'>CLOUD</b:widget-setting>
              <b:widget-setting name='selectedLabelsList'></b:widget-setting>
              <b:widget-setting name='showType'>ALL</b:widget-setting>
              <b:widget-setting name='showFreqNumbers'>false</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='cloud'>
      <ul class='cloud-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name btn' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
            <b:includable id='content'>
      <div class='widget-content'>
        <b:class expr:name='data:this.display + &quot;-label&quot;'/>
        <b:include cond='data:this.display == &quot;list&quot;' name='list'/>
        <b:include cond='data:this.display == &quot;cloud&quot;' name='cloud'/>
      </div>
    </b:includable>
            <b:includable id='list'>
      <ul class='list-style'>
        <b:loop values='data:labels' var='label'>
          <li><a class='label-name' expr:href='data:label.url'><data:label.name/><b:if cond='data:this.showFreqNumbers'><b:class name='has-count'/><span class='label-count count-style'>(<data:label.count/>)</span></b:if></a></li>
        </b:loop>
      </ul>
    </b:includable>
          </b:widget>
        </b:section>
      </aside>
    </div>
  </div>
  <b:if cond='data:view.isLayoutMode or (data:view.isHomepage and (data:widgets any w =&gt; w.sectionId == &quot;footer-ads&quot;)) or (data:view.isPost and (data:skin.vars.footerad_onpost == &quot;1px&quot;) and (data:widgets any w =&gt; w.sectionId == &quot;footer-ads&quot;))'>
    <!-- Footer Ads -->
    <div class='flex-center' id='footer-ads-wrap'>
      <b:section class='footer-ads container row-x1' id='footer-ads' maxwidgets='1' name='Footer ADS' showaddelement='yes'>
        <b:widget id='HTML33' locked='false' title='' type='HTML' visible='true'>
          <b:widget-settings>
            <b:widget-setting name='content'><![CDATA[<a class="ads-here" href="https://www.truyenmahot.com/">Liên hệ Quảng Cáo</a>]]></b:widget-setting>
          </b:widget-settings>
          <b:includable id='main'>
      <b:include name='html-content'/>
    </b:includable>
        </b:widget>
      </b:section>
    </div>
  </b:if>
  <!-- Footer Wrapper -->
  <footer id='footer-wrapper'>
    <div class='primary-footer flex-center'>
      <b:class cond='data:widgets none w =&gt; w.sectionId == &quot;litespot-pro-about-section&quot;' name='no-widget'/>
      <div class='container row-x1'>
        <b:section class='litespot-pro-about-section' id='litespot-pro-about-section' maxwidgets='2' name='About Section' showaddelement='yes'>
          <b:widget id='Image101' locked='true' title='About Us' type='Image' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='displayUrl'>https://lh6.googleusercontent.com/-OG_4FKJw9bw/YH7xl5KCpCI/AAAAAAAAAQA/X-i-eccUmHQDpzVU1g5If8yqclrIYGxQACLcBGAsYHQ/s0/logo.png</b:widget-setting>
              <b:widget-setting name='displayHeight'>60</b:widget-setting>
              <b:widget-setting name='sectionWidth'>150</b:widget-setting>
              <b:widget-setting name='shrinkToFit'>false</b:widget-setting>
              <b:widget-setting name='displayWidth'>221</b:widget-setting>
              <b:widget-setting name='link'>/</b:widget-setting>
              <b:widget-setting name='caption'><![CDATA[Chuyên trang chia sẻ truyện audio tiên hiệp, xuyên không, dị giới, kiếm hiệp, trọng sinh, ngôn tình, đô thị full hay và mới nhất.]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='image-content'/>
    </b:includable>
          </b:widget>
          <b:widget id='LinkList103' locked='true' title='Theo dõi kênh' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>https://www.instagram.com/truyenmahot</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='link-4'>/p/sitemap.html</b:widget-setting>
              <b:widget-setting name='text-1'>twitter</b:widget-setting>
              <b:widget-setting name='link-1'>https://www.twitter.com/truyenmahot</b:widget-setting>
              <b:widget-setting name='text-0'>facebook</b:widget-setting>
              <b:widget-setting name='link-2'>https://www.youtube.com/c/BaoAnTV?sub_confirmation=1</b:widget-setting>
              <b:widget-setting name='text-3'>instagram</b:widget-setting>
              <b:widget-setting name='link-0'>https://www.facebook.com/truyenmahot</b:widget-setting>
              <b:widget-setting name='text-2'>youtube</b:widget-setting>
              <b:widget-setting name='text-4'>rss</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </div>
    </div>
    <div class='footerbar flex-center'>
      <div class='container row-x1'>
        <b:section class='footer-copyright' id='footer-copyright' maxwidgets='1' name='Footer Copyright' showaddelement='yes'>
          <b:widget id='Text101' locked='true' title='' type='Text' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[Copyright &#169; <span itemprop='copyrightYear'><script>document.write((new Date()).getFullYear());</script></span> by <a href='/' rel='dofollow' style='visibility: visible;' title='Đọc Truyện Online'>Đọc Truyện Online</a>]]></b:widget-setting>
            </b:widget-settings>
            <b:includable id='main'>
              <b:include name='text-content'/>
            </b:includable>
          </b:widget>
        </b:section>
        <b:section class='footer-menu' id='footer-menu' maxwidgets='1' name='Footer Menu' showaddelement='yes'>
          <b:widget id='LinkList104' locked='true' title='Link List' type='LinkList' visible='true'>
            <b:widget-settings>
              <b:widget-setting name='link-3'>/p/shortcodes.html</b:widget-setting>
              <b:widget-setting name='sorting'>NONE</b:widget-setting>
              <b:widget-setting name='text-1'>Liên Hệ</b:widget-setting>
              <b:widget-setting name='link-1'>/p/contact.html</b:widget-setting>
              <b:widget-setting name='text-0'>Giới Thiệu</b:widget-setting>
              <b:widget-setting name='link-2'>/p/privacy.html</b:widget-setting>
              <b:widget-setting name='text-3'>Shortcodes</b:widget-setting>
              <b:widget-setting name='link-0'>/p/about.html</b:widget-setting>
              <b:widget-setting name='text-2'>Chính Sách</b:widget-setting>
            </b:widget-settings>
            <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
            <b:includable id='content'>
      <b:include name='linklist-content'/>
    </b:includable>
          </b:widget>
        </b:section>
      </div>
    </div>
  </footer>
  <b:if cond='data:view.isLayoutMode or (data:widgets.Text any w =&gt; w.sectionId == &quot;litespot-pro-cookie-ify-section&quot;)'>
      <!-- Cookie Consent -->
      <div id='litespot-pro-cookie-ify'>
          <b:section id='litespot-pro-cookie-ify-section' maxwidgets='1' name='Cookie Consent' showaddelement='no'>
          <b:widget id='Text1' locked='true' title='$ok={Accept !} $days={7}' type='Text' visible='false'>
              <b:widget-settings>
              <b:widget-setting name='content'><![CDATA[Trang web của chúng tôi sử dụng cookie để cải thiện trải nghiệm của bạn. <a href="#">Tìm hiểu thêm.</a>]]></b:widget-setting>
              </b:widget-settings>
              <b:includable id='main'>
          <b:include name='text-content'/>
      </b:includable>
          </b:widget>
          </b:section>
      </div>
  </b:if>
</div>
<!-- Mobile Menu and Back Top -->
<div id='slide-menu'>
  <div class='slide-menu-header'>
    <div class='mobile-search'>
      <form class='search-form' expr:action='data:blog.searchUrl' role='search'>
        <input autocomplete='off' class='search-input' expr:placeholder='data:messages.search' name='q' type='search' value=''/>
        <button class='search-action' type='submit' value=''/>
      </form>
    </div>
    <a class='hide-litespot-pro-mobile-menu' href='javascript:;' role='button'/>
  </div>
  <div class='slide-menu-flex'>
    <div class='litespot-pro-mobile-menu' id='litespot-pro-mobile-menu'/>
    <div class='mm-footer'>
      <div class='mm-social'/>
      <div class='mm-menu'/>
    </div>
  </div>
</div>
<div class='overlay'/>
<a class='btn' href='javascript:;' id='back-top' role='button' title='Back To Top'/>
<b:if cond='data:view.isSingleItem'>
<!-- Hidden Widgets -->
<div id='hidden-widgets-wrap' style='display:none'>
  <b:section class='hidden-widgets' deleted='true' id='hidden-widgets' maxwidgets='1' showaddelement='no'>
    <b:widget id='ContactForm1' locked='true' title='Contact Form' type='ContactForm' visible='true'>
      <b:includable id='main' var='this'>
      <b:include name='widget-title'/>
      <b:include name='content'/>
    </b:includable>
      <b:includable id='content'>
      <b:include name='contact-form-content'/>
    </b:includable>
    </b:widget>
  </b:section>
</div>
</b:if>
<b:include name='theme-options-js'/>
<!-- Local Plugins -->
<script type='text/javascript'>
//<![CDATA[
/*! jQuery v3.5.1 | (c) JS Foundation and other contributors | jquery.org/license */
!function(e,t){"use strict";"object"==typeof module&&"object"==typeof module.exports?module.exports=e.document?t(e,!0):function(e){if(!e.document)throw new Error("jQuery requires a window with a document");return t(e)}:t(e)}("undefined"!=typeof window?window:this,function(C,e){"use strict";var t=[],r=Object.getPrototypeOf,s=t.slice,g=t.flat?function(e){return t.flat.call(e)}:function(e){return t.concat.apply([],e)},u=t.push,i=t.indexOf,n={},o=n.toString,v=n.hasOwnProperty,a=v.toString,l=a.call(Object),y={},m=function(e){return"function"==typeof e&&"number"!=typeof e.nodeType},x=function(e){return null!=e&&e===e.window},E=C.document,c={type:!0,src:!0,nonce:!0,noModule:!0};function b(e,t,n){var r,i,o=(n=n||E).createElement("script");if(o.text=e,t)for(r in c)(i=t[r]||t.getAttribute&&t.getAttribute(r))&&o.setAttribute(r,i);n.head.appendChild(o).parentNode.removeChild(o)}function w(e){return null==e?e+"":"object"==typeof e||"function"==typeof e?n[o.call(e)]||"object":typeof e}var f="3.5.1",S=function(e,t){return new S.fn.init(e,t)};function p(e){var t=!!e&&"length"in e&&e.length,n=w(e);return!m(e)&&!x(e)&&("array"===n||0===t||"number"==typeof t&&0<t&&t-1 in e)}S.fn=S.prototype={jquery:f,constructor:S,length:0,toArray:function(){return s.call(this)},get:function(e){return null==e?s.call(this):e<0?this[e+this.length]:this[e]},pushStack:function(e){var t=S.merge(this.constructor(),e);return t.prevObject=this,t},each:function(e){return S.each(this,e)},map:function(n){return this.pushStack(S.map(this,function(e,t){return n.call(e,t,e)}))},slice:function(){return this.pushStack(s.apply(this,arguments))},first:function(){return this.eq(0)},last:function(){return this.eq(-1)},even:function(){return this.pushStack(S.grep(this,function(e,t){return(t+1)%2}))},odd:function(){return this.pushStack(S.grep(this,function(e,t){return t%2}))},eq:function(e){var t=this.length,n=+e+(e<0?t:0);return this.pushStack(0<=n&&n<t?[this[n]]:[])},end:function(){return this.prevObject||this.constructor()},push:u,sort:t.sort,splice:t.splice},S.extend=S.fn.extend=function(){var e,t,n,r,i,o,a=arguments[0]||{},s=1,u=arguments.length,l=!1;for("boolean"==typeof a&&(l=a,a=arguments[s]||{},s++),"object"==typeof a||m(a)||(a={}),s===u&&(a=this,s--);s<u;s++)if(null!=(e=arguments[s]))for(t in e)r=e[t],"__proto__"!==t&&a!==r&&(l&&r&&(S.isPlainObject(r)||(i=Array.isArray(r)))?(n=a[t],o=i&&!Array.isArray(n)?[]:i||S.isPlainObject(n)?n:{},i=!1,a[t]=S.extend(l,o,r)):void 0!==r&&(a[t]=r));return a},S.extend({expando:"jQuery"+(f+Math.random()).replace(/\D/g,""),isReady:!0,error:function(e){throw new Error(e)},noop:function(){},isPlainObject:function(e){var t,n;return!(!e||"[object Object]"!==o.call(e))&&(!(t=r(e))||"function"==typeof(n=v.call(t,"constructor")&&t.constructor)&&a.call(n)===l)},isEmptyObject:function(e){var t;for(t in e)return!1;return!0},globalEval:function(e,t,n){b(e,{nonce:t&&t.nonce},n)},each:function(e,t){var n,r=0;if(p(e)){for(n=e.length;r<n;r++)if(!1===t.call(e[r],r,e[r]))break}else for(r in e)if(!1===t.call(e[r],r,e[r]))break;return e},makeArray:function(e,t){var n=t||[];return null!=e&&(p(Object(e))?S.merge(n,"string"==typeof e?[e]:e):u.call(n,e)),n},inArray:function(e,t,n){return null==t?-1:i.call(t,e,n)},merge:function(e,t){for(var n=+t.length,r=0,i=e.length;r<n;r++)e[i++]=t[r];return e.length=i,e},grep:function(e,t,n){for(var r=[],i=0,o=e.length,a=!n;i<o;i++)!t(e[i],i)!==a&&r.push(e[i]);return r},map:function(e,t,n){var r,i,o=0,a=[];if(p(e))for(r=e.length;o<r;o++)null!=(i=t(e[o],o,n))&&a.push(i);else for(o in e)null!=(i=t(e[o],o,n))&&a.push(i);return g(a)},guid:1,support:y}),"function"==typeof Symbol&&(S.fn[Symbol.iterator]=t[Symbol.iterator]),S.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "),function(e,t){n["[object "+t+"]"]=t.toLowerCase()});var d=function(n){var e,d,b,o,i,h,f,g,w,u,l,T,C,a,E,v,s,c,y,S="sizzle"+1*new Date,p=n.document,k=0,r=0,m=ue(),x=ue(),A=ue(),N=ue(),D=function(e,t){return e===t&&(l=!0),0},j={}.hasOwnProperty,t=[],q=t.pop,L=t.push,H=t.push,O=t.slice,P=function(e,t){for(var n=0,r=e.length;n<r;n++)if(e[n]===t)return n;return-1},R="checked|selected|async|autofocus|autoplay|controls|defer|disabled|hidden|ismap|loop|multiple|open|readonly|required|scoped",M="[\\x20\\t\\r\\n\\f]",I="(?:\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\[^\\r\\n\\f]|[\\w-]|[^\0-\\x7f])+",W="\\["+M+"*("+I+")(?:"+M+"*([*^$|!~]?=)"+M+"*(?:'((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\"|("+I+"))|)"+M+"*\\]",F=":("+I+")(?:\\((('((?:\\\\.|[^\\\\'])*)'|\"((?:\\\\.|[^\\\\\"])*)\")|((?:\\\\.|[^\\\\()[\\]]|"+W+")*)|.*)\\)|)",B=new RegExp(M+"+","g"),$=new RegExp("^"+M+"+|((?:^|[^\\\\])(?:\\\\.)*)"+M+"+$","g"),_=new RegExp("^"+M+"*,"+M+"*"),z=new RegExp("^"+M+"*([>+~]|"+M+")"+M+"*"),U=new RegExp(M+"|>"),X=new RegExp(F),V=new RegExp("^"+I+"$"),G={ID:new RegExp("^#("+I+")"),CLASS:new RegExp("^\\.("+I+")"),TAG:new RegExp("^("+I+"|[*])"),ATTR:new RegExp("^"+W),PSEUDO:new RegExp("^"+F),CHILD:new RegExp("^:(only|first|last|nth|nth-last)-(child|of-type)(?:\\("+M+"*(even|odd|(([+-]|)(\\d*)n|)"+M+"*(?:([+-]|)"+M+"*(\\d+)|))"+M+"*\\)|)","i"),bool:new RegExp("^(?:"+R+")$","i"),needsContext:new RegExp("^"+M+"*[>+~]|:(even|odd|eq|gt|lt|nth|first|last)(?:\\("+M+"*((?:-\\d)?\\d*)"+M+"*\\)|)(?=[^-]|$)","i")},Y=/HTML$/i,Q=/^(?:input|select|textarea|button)$/i,J=/^h\d$/i,K=/^[^{]+\{\s*\[native \w/,Z=/^(?:#([\w-]+)|(\w+)|\.([\w-]+))$/,ee=/[+~]/,te=new RegExp("\\\\[\\da-fA-F]{1,6}"+M+"?|\\\\([^\\r\\n\\f])","g"),ne=function(e,t){var n="0x"+e.slice(1)-65536;return t||(n<0?String.fromCharCode(n+65536):String.fromCharCode(n>>10|55296,1023&n|56320))},re=/([\0-\x1f\x7f]|^-?\d)|^-$|[^\0-\x1f\x7f-\uFFFF\w-]/g,ie=function(e,t){return t?"\0"===e?"\ufffd":e.slice(0,-1)+"\\"+e.charCodeAt(e.length-1).toString(16)+" ":"\\"+e},oe=function(){T()},ae=be(function(e){return!0===e.disabled&&"fieldset"===e.nodeName.toLowerCase()},{dir:"parentNode",next:"legend"});try{H.apply(t=O.call(p.childNodes),p.childNodes),t[p.childNodes.length].nodeType}catch(e){H={apply:t.length?function(e,t){L.apply(e,O.call(t))}:function(e,t){var n=e.length,r=0;while(e[n++]=t[r++]);e.length=n-1}}}function se(t,e,n,r){var i,o,a,s,u,l,c,f=e&&e.ownerDocument,p=e?e.nodeType:9;if(n=n||[],"string"!=typeof t||!t||1!==p&&9!==p&&11!==p)return n;if(!r&&(T(e),e=e||C,E)){if(11!==p&&(u=Z.exec(t)))if(i=u[1]){if(9===p){if(!(a=e.getElementById(i)))return n;if(a.id===i)return n.push(a),n}else if(f&&(a=f.getElementById(i))&&y(e,a)&&a.id===i)return n.push(a),n}else{if(u[2])return H.apply(n,e.getElementsByTagName(t)),n;if((i=u[3])&&d.getElementsByClassName&&e.getElementsByClassName)return H.apply(n,e.getElementsByClassName(i)),n}if(d.qsa&&!N[t+" "]&&(!v||!v.test(t))&&(1!==p||"object"!==e.nodeName.toLowerCase())){if(c=t,f=e,1===p&&(U.test(t)||z.test(t))){(f=ee.test(t)&&ye(e.parentNode)||e)===e&&d.scope||((s=e.getAttribute("id"))?s=s.replace(re,ie):e.setAttribute("id",s=S)),o=(l=h(t)).length;while(o--)l[o]=(s?"#"+s:":scope")+" "+xe(l[o]);c=l.join(",")}try{return H.apply(n,f.querySelectorAll(c)),n}catch(e){N(t,!0)}finally{s===S&&e.removeAttribute("id")}}}return g(t.replace($,"$1"),e,n,r)}function ue(){var r=[];return function e(t,n){return r.push(t+" ")>b.cacheLength&&delete e[r.shift()],e[t+" "]=n}}function le(e){return e[S]=!0,e}function ce(e){var t=C.createElement("fieldset");try{return!!e(t)}catch(e){return!1}finally{t.parentNode&&t.parentNode.removeChild(t),t=null}}function fe(e,t){var n=e.split("|"),r=n.length;while(r--)b.attrHandle[n[r]]=t}function pe(e,t){var n=t&&e,r=n&&1===e.nodeType&&1===t.nodeType&&e.sourceIndex-t.sourceIndex;if(r)return r;if(n)while(n=n.nextSibling)if(n===t)return-1;return e?1:-1}function de(t){return function(e){return"input"===e.nodeName.toLowerCase()&&e.type===t}}function he(n){return function(e){var t=e.nodeName.toLowerCase();return("input"===t||"button"===t)&&e.type===n}}function ge(t){return function(e){return"form"in e?e.parentNode&&!1===e.disabled?"label"in e?"label"in e.parentNode?e.parentNode.disabled===t:e.disabled===t:e.isDisabled===t||e.isDisabled!==!t&&ae(e)===t:e.disabled===t:"label"in e&&e.disabled===t}}function ve(a){return le(function(o){return o=+o,le(function(e,t){var n,r=a([],e.length,o),i=r.length;while(i--)e[n=r[i]]&&(e[n]=!(t[n]=e[n]))})})}function ye(e){return e&&"undefined"!=typeof e.getElementsByTagName&&e}for(e in d=se.support={},i=se.isXML=function(e){var t=e.namespaceURI,n=(e.ownerDocument||e).documentElement;return!Y.test(t||n&&n.nodeName||"HTML")},T=se.setDocument=function(e){var t,n,r=e?e.ownerDocument||e:p;return r!=C&&9===r.nodeType&&r.documentElement&&(a=(C=r).documentElement,E=!i(C),p!=C&&(n=C.defaultView)&&n.top!==n&&(n.addEventListener?n.addEventListener("unload",oe,!1):n.attachEvent&&n.attachEvent("onunload",oe)),d.scope=ce(function(e){return a.appendChild(e).appendChild(C.createElement("div")),"undefined"!=typeof e.querySelectorAll&&!e.querySelectorAll(":scope fieldset div").length}),d.attributes=ce(function(e){return e.className="i",!e.getAttribute("className")}),d.getElementsByTagName=ce(function(e){return e.appendChild(C.createComment("")),!e.getElementsByTagName("*").length}),d.getElementsByClassName=K.test(C.getElementsByClassName),d.getById=ce(function(e){return a.appendChild(e).id=S,!C.getElementsByName||!C.getElementsByName(S).length}),d.getById?(b.filter.ID=function(e){var t=e.replace(te,ne);return function(e){return e.getAttribute("id")===t}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n=t.getElementById(e);return n?[n]:[]}}):(b.filter.ID=function(e){var n=e.replace(te,ne);return function(e){var t="undefined"!=typeof e.getAttributeNode&&e.getAttributeNode("id");return t&&t.value===n}},b.find.ID=function(e,t){if("undefined"!=typeof t.getElementById&&E){var n,r,i,o=t.getElementById(e);if(o){if((n=o.getAttributeNode("id"))&&n.value===e)return[o];i=t.getElementsByName(e),r=0;while(o=i[r++])if((n=o.getAttributeNode("id"))&&n.value===e)return[o]}return[]}}),b.find.TAG=d.getElementsByTagName?function(e,t){return"undefined"!=typeof t.getElementsByTagName?t.getElementsByTagName(e):d.qsa?t.querySelectorAll(e):void 0}:function(e,t){var n,r=[],i=0,o=t.getElementsByTagName(e);if("*"===e){while(n=o[i++])1===n.nodeType&&r.push(n);return r}return o},b.find.CLASS=d.getElementsByClassName&&function(e,t){if("undefined"!=typeof t.getElementsByClassName&&E)return t.getElementsByClassName(e)},s=[],v=[],(d.qsa=K.test(C.querySelectorAll))&&(ce(function(e){var t;a.appendChild(e).innerHTML="<a id='"+S+"'></a><select id='"+S+"-\r\\' msallowcapture=''><option selected=''></option></select>",e.querySelectorAll("[msallowcapture^='']").length&&v.push("[*^$]="+M+"*(?:''|\"\")"),e.querySelectorAll("[selected]").length||v.push("\\["+M+"*(?:value|"+R+")"),e.querySelectorAll("[id~="+S+"-]").length||v.push("~="),(t=C.createElement("input")).setAttribute("name",""),e.appendChild(t),e.querySelectorAll("[name='']").length||v.push("\\["+M+"*name"+M+"*="+M+"*(?:''|\"\")"),e.querySelectorAll(":checked").length||v.push(":checked"),e.querySelectorAll("a#"+S+"+*").length||v.push(".#.+[+~]"),e.querySelectorAll("\\\f"),v.push("[\\r\\n\\f]")}),ce(function(e){e.innerHTML="<a href='' disabled='disabled'></a><select disabled='disabled'><option/></select>";var t=C.createElement("input");t.setAttribute("type","hidden"),e.appendChild(t).setAttribute("name","D"),e.querySelectorAll("[name=d]").length&&v.push("name"+M+"*[*^$|!~]?="),2!==e.querySelectorAll(":enabled").length&&v.push(":enabled",":disabled"),a.appendChild(e).disabled=!0,2!==e.querySelectorAll(":disabled").length&&v.push(":enabled",":disabled"),e.querySelectorAll("*,:x"),v.push(",.*:")})),(d.matchesSelector=K.test(c=a.matches||a.webkitMatchesSelector||a.mozMatchesSelector||a.oMatchesSelector||a.msMatchesSelector))&&ce(function(e){d.disconnectedMatch=c.call(e,"*"),c.call(e,"[s!='']:x"),s.push("!=",F)}),v=v.length&&new RegExp(v.join("|")),s=s.length&&new RegExp(s.join("|")),t=K.test(a.compareDocumentPosition),y=t||K.test(a.contains)?function(e,t){var n=9===e.nodeType?e.documentElement:e,r=t&&t.parentNode;return e===r||!(!r||1!==r.nodeType||!(n.contains?n.contains(r):e.compareDocumentPosition&&16&e.compareDocumentPosition(r)))}:function(e,t){if(t)while(t=t.parentNode)if(t===e)return!0;return!1},D=t?function(e,t){if(e===t)return l=!0,0;var n=!e.compareDocumentPosition-!t.compareDocumentPosition;return n||(1&(n=(e.ownerDocument||e)==(t.ownerDocument||t)?e.compareDocumentPosition(t):1)||!d.sortDetached&&t.compareDocumentPosition(e)===n?e==C||e.ownerDocument==p&&y(p,e)?-1:t==C||t.ownerDocument==p&&y(p,t)?1:u?P(u,e)-P(u,t):0:4&n?-1:1)}:function(e,t){if(e===t)return l=!0,0;var n,r=0,i=e.parentNode,o=t.parentNode,a=[e],s=[t];if(!i||!o)return e==C?-1:t==C?1:i?-1:o?1:u?P(u,e)-P(u,t):0;if(i===o)return pe(e,t);n=e;while(n=n.parentNode)a.unshift(n);n=t;while(n=n.parentNode)s.unshift(n);while(a[r]===s[r])r++;return r?pe(a[r],s[r]):a[r]==p?-1:s[r]==p?1:0}),C},se.matches=function(e,t){return se(e,null,null,t)},se.matchesSelector=function(e,t){if(T(e),d.matchesSelector&&E&&!N[t+" "]&&(!s||!s.test(t))&&(!v||!v.test(t)))try{var n=c.call(e,t);if(n||d.disconnectedMatch||e.document&&11!==e.document.nodeType)return n}catch(e){N(t,!0)}return 0<se(t,C,null,[e]).length},se.contains=function(e,t){return(e.ownerDocument||e)!=C&&T(e),y(e,t)},se.attr=function(e,t){(e.ownerDocument||e)!=C&&T(e);var n=b.attrHandle[t.toLowerCase()],r=n&&j.call(b.attrHandle,t.toLowerCase())?n(e,t,!E):void 0;return void 0!==r?r:d.attributes||!E?e.getAttribute(t):(r=e.getAttributeNode(t))&&r.specified?r.value:null},se.escape=function(e){return(e+"").replace(re,ie)},se.error=function(e){throw new Error("Syntax error, unrecognized expression: "+e)},se.uniqueSort=function(e){var t,n=[],r=0,i=0;if(l=!d.detectDuplicates,u=!d.sortStable&&e.slice(0),e.sort(D),l){while(t=e[i++])t===e[i]&&(r=n.push(i));while(r--)e.splice(n[r],1)}return u=null,e},o=se.getText=function(e){var t,n="",r=0,i=e.nodeType;if(i){if(1===i||9===i||11===i){if("string"==typeof e.textContent)return e.textContent;for(e=e.firstChild;e;e=e.nextSibling)n+=o(e)}else if(3===i||4===i)return e.nodeValue}else while(t=e[r++])n+=o(t);return n},(b=se.selectors={cacheLength:50,createPseudo:le,match:G,attrHandle:{},find:{},relative:{">":{dir:"parentNode",first:!0}," ":{dir:"parentNode"},"+":{dir:"previousSibling",first:!0},"~":{dir:"previousSibling"}},preFilter:{ATTR:function(e){return e[1]=e[1].replace(te,ne),e[3]=(e[3]||e[4]||e[5]||"").replace(te,ne),"~="===e[2]&&(e[3]=" "+e[3]+" "),e.slice(0,4)},CHILD:function(e){return e[1]=e[1].toLowerCase(),"nth"===e[1].slice(0,3)?(e[3]||se.error(e[0]),e[4]=+(e[4]?e[5]+(e[6]||1):2*("even"===e[3]||"odd"===e[3])),e[5]=+(e[7]+e[8]||"odd"===e[3])):e[3]&&se.error(e[0]),e},PSEUDO:function(e){var t,n=!e[6]&&e[2];return G.CHILD.test(e[0])?null:(e[3]?e[2]=e[4]||e[5]||"":n&&X.test(n)&&(t=h(n,!0))&&(t=n.indexOf(")",n.length-t)-n.length)&&(e[0]=e[0].slice(0,t),e[2]=n.slice(0,t)),e.slice(0,3))}},filter:{TAG:function(e){var t=e.replace(te,ne).toLowerCase();return"*"===e?function(){return!0}:function(e){return e.nodeName&&e.nodeName.toLowerCase()===t}},CLASS:function(e){var t=m[e+" "];return t||(t=new RegExp("(^|"+M+")"+e+"("+M+"|$)"))&&m(e,function(e){return t.test("string"==typeof e.className&&e.className||"undefined"!=typeof e.getAttribute&&e.getAttribute("class")||"")})},ATTR:function(n,r,i){return function(e){var t=se.attr(e,n);return null==t?"!="===r:!r||(t+="","="===r?t===i:"!="===r?t!==i:"^="===r?i&&0===t.indexOf(i):"*="===r?i&&-1<t.indexOf(i):"$="===r?i&&t.slice(-i.length)===i:"~="===r?-1<(" "+t.replace(B," ")+" ").indexOf(i):"|="===r&&(t===i||t.slice(0,i.length+1)===i+"-"))}},CHILD:function(h,e,t,g,v){var y="nth"!==h.slice(0,3),m="last"!==h.slice(-4),x="of-type"===e;return 1===g&&0===v?function(e){return!!e.parentNode}:function(e,t,n){var r,i,o,a,s,u,l=y!==m?"nextSibling":"previousSibling",c=e.parentNode,f=x&&e.nodeName.toLowerCase(),p=!n&&!x,d=!1;if(c){if(y){while(l){a=e;while(a=a[l])if(x?a.nodeName.toLowerCase()===f:1===a.nodeType)return!1;u=l="only"===h&&!u&&"nextSibling"}return!0}if(u=[m?c.firstChild:c.lastChild],m&&p){d=(s=(r=(i=(o=(a=c)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1])&&r[2],a=s&&c.childNodes[s];while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if(1===a.nodeType&&++d&&a===e){i[h]=[k,s,d];break}}else if(p&&(d=s=(r=(i=(o=(a=e)[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]||[])[0]===k&&r[1]),!1===d)while(a=++s&&a&&a[l]||(d=s=0)||u.pop())if((x?a.nodeName.toLowerCase()===f:1===a.nodeType)&&++d&&(p&&((i=(o=a[S]||(a[S]={}))[a.uniqueID]||(o[a.uniqueID]={}))[h]=[k,d]),a===e))break;return(d-=v)===g||d%g==0&&0<=d/g}}},PSEUDO:function(e,o){var t,a=b.pseudos[e]||b.setFilters[e.toLowerCase()]||se.error("unsupported pseudo: "+e);return a[S]?a(o):1<a.length?(t=[e,e,"",o],b.setFilters.hasOwnProperty(e.toLowerCase())?le(function(e,t){var n,r=a(e,o),i=r.length;while(i--)e[n=P(e,r[i])]=!(t[n]=r[i])}):function(e){return a(e,0,t)}):a}},pseudos:{not:le(function(e){var r=[],i=[],s=f(e.replace($,"$1"));return s[S]?le(function(e,t,n,r){var i,o=s(e,null,r,[]),a=e.length;while(a--)(i=o[a])&&(e[a]=!(t[a]=i))}):function(e,t,n){return r[0]=e,s(r,null,n,i),r[0]=null,!i.pop()}}),has:le(function(t){return function(e){return 0<se(t,e).length}}),contains:le(function(t){return t=t.replace(te,ne),function(e){return-1<(e.textContent||o(e)).indexOf(t)}}),lang:le(function(n){return V.test(n||"")||se.error("unsupported lang: "+n),n=n.replace(te,ne).toLowerCase(),function(e){var t;do{if(t=E?e.lang:e.getAttribute("xml:lang")||e.getAttribute("lang"))return(t=t.toLowerCase())===n||0===t.indexOf(n+"-")}while((e=e.parentNode)&&1===e.nodeType);return!1}}),target:function(e){var t=n.location&&n.location.hash;return t&&t.slice(1)===e.id},root:function(e){return e===a},focus:function(e){return e===C.activeElement&&(!C.hasFocus||C.hasFocus())&&!!(e.type||e.href||~e.tabIndex)},enabled:ge(!1),disabled:ge(!0),checked:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&!!e.checked||"option"===t&&!!e.selected},selected:function(e){return e.parentNode&&e.parentNode.selectedIndex,!0===e.selected},empty:function(e){for(e=e.firstChild;e;e=e.nextSibling)if(e.nodeType<6)return!1;return!0},parent:function(e){return!b.pseudos.empty(e)},header:function(e){return J.test(e.nodeName)},input:function(e){return Q.test(e.nodeName)},button:function(e){var t=e.nodeName.toLowerCase();return"input"===t&&"button"===e.type||"button"===t},text:function(e){var t;return"input"===e.nodeName.toLowerCase()&&"text"===e.type&&(null==(t=e.getAttribute("type"))||"text"===t.toLowerCase())},first:ve(function(){return[0]}),last:ve(function(e,t){return[t-1]}),eq:ve(function(e,t,n){return[n<0?n+t:n]}),even:ve(function(e,t){for(var n=0;n<t;n+=2)e.push(n);return e}),odd:ve(function(e,t){for(var n=1;n<t;n+=2)e.push(n);return e}),lt:ve(function(e,t,n){for(var r=n<0?n+t:t<n?t:n;0<=--r;)e.push(r);return e}),gt:ve(function(e,t,n){for(var r=n<0?n+t:n;++r<t;)e.push(r);return e})}}).pseudos.nth=b.pseudos.eq,{radio:!0,checkbox:!0,file:!0,password:!0,image:!0})b.pseudos[e]=de(e);for(e in{submit:!0,reset:!0})b.pseudos[e]=he(e);function me(){}function xe(e){for(var t=0,n=e.length,r="";t<n;t++)r+=e[t].value;return r}function be(s,e,t){var u=e.dir,l=e.next,c=l||u,f=t&&"parentNode"===c,p=r++;return e.first?function(e,t,n){while(e=e[u])if(1===e.nodeType||f)return s(e,t,n);return!1}:function(e,t,n){var r,i,o,a=[k,p];if(n){while(e=e[u])if((1===e.nodeType||f)&&s(e,t,n))return!0}else while(e=e[u])if(1===e.nodeType||f)if(i=(o=e[S]||(e[S]={}))[e.uniqueID]||(o[e.uniqueID]={}),l&&l===e.nodeName.toLowerCase())e=e[u]||e;else{if((r=i[c])&&r[0]===k&&r[1]===p)return a[2]=r[2];if((i[c]=a)[2]=s(e,t,n))return!0}return!1}}function we(i){return 1<i.length?function(e,t,n){var r=i.length;while(r--)if(!i[r](e,t,n))return!1;return!0}:i[0]}function Te(e,t,n,r,i){for(var o,a=[],s=0,u=e.length,l=null!=t;s<u;s++)(o=e[s])&&(n&&!n(o,r,i)||(a.push(o),l&&t.push(s)));return a}function Ce(d,h,g,v,y,e){return v&&!v[S]&&(v=Ce(v)),y&&!y[S]&&(y=Ce(y,e)),le(function(e,t,n,r){var i,o,a,s=[],u=[],l=t.length,c=e||function(e,t,n){for(var r=0,i=t.length;r<i;r++)se(e,t[r],n);return n}(h||"*",n.nodeType?[n]:n,[]),f=!d||!e&&h?c:Te(c,s,d,n,r),p=g?y||(e?d:l||v)?[]:t:f;if(g&&g(f,p,n,r),v){i=Te(p,u),v(i,[],n,r),o=i.length;while(o--)(a=i[o])&&(p[u[o]]=!(f[u[o]]=a))}if(e){if(y||d){if(y){i=[],o=p.length;while(o--)(a=p[o])&&i.push(f[o]=a);y(null,p=[],i,r)}o=p.length;while(o--)(a=p[o])&&-1<(i=y?P(e,a):s[o])&&(e[i]=!(t[i]=a))}}else p=Te(p===t?p.splice(l,p.length):p),y?y(null,t,p,r):H.apply(t,p)})}function Ee(e){for(var i,t,n,r=e.length,o=b.relative[e[0].type],a=o||b.relative[" "],s=o?1:0,u=be(function(e){return e===i},a,!0),l=be(function(e){return-1<P(i,e)},a,!0),c=[function(e,t,n){var r=!o&&(n||t!==w)||((i=t).nodeType?u(e,t,n):l(e,t,n));return i=null,r}];s<r;s++)if(t=b.relative[e[s].type])c=[be(we(c),t)];else{if((t=b.filter[e[s].type].apply(null,e[s].matches))[S]){for(n=++s;n<r;n++)if(b.relative[e[n].type])break;return Ce(1<s&&we(c),1<s&&xe(e.slice(0,s-1).concat({value:" "===e[s-2].type?"*":""})).replace($,"$1"),t,s<n&&Ee(e.slice(s,n)),n<r&&Ee(e=e.slice(n)),n<r&&xe(e))}c.push(t)}return we(c)}return me.prototype=b.filters=b.pseudos,b.setFilters=new me,h=se.tokenize=function(e,t){var n,r,i,o,a,s,u,l=x[e+" "];if(l)return t?0:l.slice(0);a=e,s=[],u=b.preFilter;while(a){for(o in n&&!(r=_.exec(a))||(r&&(a=a.slice(r[0].length)||a),s.push(i=[])),n=!1,(r=z.exec(a))&&(n=r.shift(),i.push({value:n,type:r[0].replace($," ")}),a=a.slice(n.length)),b.filter)!(r=G[o].exec(a))||u[o]&&!(r=u[o](r))||(n=r.shift(),i.push({value:n,type:o,matches:r}),a=a.slice(n.length));if(!n)break}return t?a.length:a?se.error(e):x(e,s).slice(0)},f=se.compile=function(e,t){var n,v,y,m,x,r,i=[],o=[],a=A[e+" "];if(!a){t||(t=h(e)),n=t.length;while(n--)(a=Ee(t[n]))[S]?i.push(a):o.push(a);(a=A(e,(v=o,m=0<(y=i).length,x=0<v.length,r=function(e,t,n,r,i){var o,a,s,u=0,l="0",c=e&&[],f=[],p=w,d=e||x&&b.find.TAG("*",i),h=k+=null==p?1:Math.random()||.1,g=d.length;for(i&&(w=t==C||t||i);l!==g&&null!=(o=d[l]);l++){if(x&&o){a=0,t||o.ownerDocument==C||(T(o),n=!E);while(s=v[a++])if(s(o,t||C,n)){r.push(o);break}i&&(k=h)}m&&((o=!s&&o)&&u--,e&&c.push(o))}if(u+=l,m&&l!==u){a=0;while(s=y[a++])s(c,f,t,n);if(e){if(0<u)while(l--)c[l]||f[l]||(f[l]=q.call(r));f=Te(f)}H.apply(r,f),i&&!e&&0<f.length&&1<u+y.length&&se.uniqueSort(r)}return i&&(k=h,w=p),c},m?le(r):r))).selector=e}return a},g=se.select=function(e,t,n,r){var i,o,a,s,u,l="function"==typeof e&&e,c=!r&&h(e=l.selector||e);if(n=n||[],1===c.length){if(2<(o=c[0]=c[0].slice(0)).length&&"ID"===(a=o[0]).type&&9===t.nodeType&&E&&b.relative[o[1].type]){if(!(t=(b.find.ID(a.matches[0].replace(te,ne),t)||[])[0]))return n;l&&(t=t.parentNode),e=e.slice(o.shift().value.length)}i=G.needsContext.test(e)?0:o.length;while(i--){if(a=o[i],b.relative[s=a.type])break;if((u=b.find[s])&&(r=u(a.matches[0].replace(te,ne),ee.test(o[0].type)&&ye(t.parentNode)||t))){if(o.splice(i,1),!(e=r.length&&xe(o)))return H.apply(n,r),n;break}}}return(l||f(e,c))(r,t,!E,n,!t||ee.test(e)&&ye(t.parentNode)||t),n},d.sortStable=S.split("").sort(D).join("")===S,d.detectDuplicates=!!l,T(),d.sortDetached=ce(function(e){return 1&e.compareDocumentPosition(C.createElement("fieldset"))}),ce(function(e){return e.innerHTML="<a href='#'></a>","#"===e.firstChild.getAttribute("href")})||fe("type|href|height|width",function(e,t,n){if(!n)return e.getAttribute(t,"type"===t.toLowerCase()?1:2)}),d.attributes&&ce(function(e){return e.innerHTML="<input/>",e.firstChild.setAttribute("value",""),""===e.firstChild.getAttribute("value")})||fe("value",function(e,t,n){if(!n&&"input"===e.nodeName.toLowerCase())return e.defaultValue}),ce(function(e){return null==e.getAttribute("disabled")})||fe(R,function(e,t,n){var r;if(!n)return!0===e[t]?t.toLowerCase():(r=e.getAttributeNode(t))&&r.specified?r.value:null}),se}(C);S.find=d,S.expr=d.selectors,S.expr[":"]=S.expr.pseudos,S.uniqueSort=S.unique=d.uniqueSort,S.text=d.getText,S.isXMLDoc=d.isXML,S.contains=d.contains,S.escapeSelector=d.escape;var h=function(e,t,n){var r=[],i=void 0!==n;while((e=e[t])&&9!==e.nodeType)if(1===e.nodeType){if(i&&S(e).is(n))break;r.push(e)}return r},T=function(e,t){for(var n=[];e;e=e.nextSibling)1===e.nodeType&&e!==t&&n.push(e);return n},k=S.expr.match.needsContext;function A(e,t){return e.nodeName&&e.nodeName.toLowerCase()===t.toLowerCase()}var N=/^<([a-z][^\/\0>:\x20\t\r\n\f]*)[\x20\t\r\n\f]*\/?>(?:<\/\1>|)$/i;function D(e,n,r){return m(n)?S.grep(e,function(e,t){return!!n.call(e,t,e)!==r}):n.nodeType?S.grep(e,function(e){return e===n!==r}):"string"!=typeof n?S.grep(e,function(e){return-1<i.call(n,e)!==r}):S.filter(n,e,r)}S.filter=function(e,t,n){var r=t[0];return n&&(e=":not("+e+")"),1===t.length&&1===r.nodeType?S.find.matchesSelector(r,e)?[r]:[]:S.find.matches(e,S.grep(t,function(e){return 1===e.nodeType}))},S.fn.extend({find:function(e){var t,n,r=this.length,i=this;if("string"!=typeof e)return this.pushStack(S(e).filter(function(){for(t=0;t<r;t++)if(S.contains(i[t],this))return!0}));for(n=this.pushStack([]),t=0;t<r;t++)S.find(e,i[t],n);return 1<r?S.uniqueSort(n):n},filter:function(e){return this.pushStack(D(this,e||[],!1))},not:function(e){return this.pushStack(D(this,e||[],!0))},is:function(e){return!!D(this,"string"==typeof e&&k.test(e)?S(e):e||[],!1).length}});var j,q=/^(?:\s*(<[\w\W]+>)[^>]*|#([\w-]+))$/;(S.fn.init=function(e,t,n){var r,i;if(!e)return this;if(n=n||j,"string"==typeof e){if(!(r="<"===e[0]&&">"===e[e.length-1]&&3<=e.length?[null,e,null]:q.exec(e))||!r[1]&&t)return!t||t.jquery?(t||n).find(e):this.constructor(t).find(e);if(r[1]){if(t=t instanceof S?t[0]:t,S.merge(this,S.parseHTML(r[1],t&&t.nodeType?t.ownerDocument||t:E,!0)),N.test(r[1])&&S.isPlainObject(t))for(r in t)m(this[r])?this[r](t[r]):this.attr(r,t[r]);return this}return(i=E.getElementById(r[2]))&&(this[0]=i,this.length=1),this}return e.nodeType?(this[0]=e,this.length=1,this):m(e)?void 0!==n.ready?n.ready(e):e(S):S.makeArray(e,this)}).prototype=S.fn,j=S(E);var L=/^(?:parents|prev(?:Until|All))/,H={children:!0,contents:!0,next:!0,prev:!0};function O(e,t){while((e=e[t])&&1!==e.nodeType);return e}S.fn.extend({has:function(e){var t=S(e,this),n=t.length;return this.filter(function(){for(var e=0;e<n;e++)if(S.contains(this,t[e]))return!0})},closest:function(e,t){var n,r=0,i=this.length,o=[],a="string"!=typeof e&&S(e);if(!k.test(e))for(;r<i;r++)for(n=this[r];n&&n!==t;n=n.parentNode)if(n.nodeType<11&&(a?-1<a.index(n):1===n.nodeType&&S.find.matchesSelector(n,e))){o.push(n);break}return this.pushStack(1<o.length?S.uniqueSort(o):o)},index:function(e){return e?"string"==typeof e?i.call(S(e),this[0]):i.call(this,e.jquery?e[0]:e):this[0]&&this[0].parentNode?this.first().prevAll().length:-1},add:function(e,t){return this.pushStack(S.uniqueSort(S.merge(this.get(),S(e,t))))},addBack:function(e){return this.add(null==e?this.prevObject:this.prevObject.filter(e))}}),S.each({parent:function(e){var t=e.parentNode;return t&&11!==t.nodeType?t:null},parents:function(e){return h(e,"parentNode")},parentsUntil:function(e,t,n){return h(e,"parentNode",n)},next:function(e){return O(e,"nextSibling")},prev:function(e){return O(e,"previousSibling")},nextAll:function(e){return h(e,"nextSibling")},prevAll:function(e){return h(e,"previousSibling")},nextUntil:function(e,t,n){return h(e,"nextSibling",n)},prevUntil:function(e,t,n){return h(e,"previousSibling",n)},siblings:function(e){return T((e.parentNode||{}).firstChild,e)},children:function(e){return T(e.firstChild)},contents:function(e){return null!=e.contentDocument&&r(e.contentDocument)?e.contentDocument:(A(e,"template")&&(e=e.content||e),S.merge([],e.childNodes))}},function(r,i){S.fn[r]=function(e,t){var n=S.map(this,i,e);return"Until"!==r.slice(-5)&&(t=e),t&&"string"==typeof t&&(n=S.filter(t,n)),1<this.length&&(H[r]||S.uniqueSort(n),L.test(r)&&n.reverse()),this.pushStack(n)}});var P=/[^\x20\t\r\n\f]+/g;function R(e){return e}function M(e){throw e}function I(e,t,n,r){var i;try{e&&m(i=e.promise)?i.call(e).done(t).fail(n):e&&m(i=e.then)?i.call(e,t,n):t.apply(void 0,[e].slice(r))}catch(e){n.apply(void 0,[e])}}S.Callbacks=function(r){var e,n;r="string"==typeof r?(e=r,n={},S.each(e.match(P)||[],function(e,t){n[t]=!0}),n):S.extend({},r);var i,t,o,a,s=[],u=[],l=-1,c=function(){for(a=a||r.once,o=i=!0;u.length;l=-1){t=u.shift();while(++l<s.length)!1===s[l].apply(t[0],t[1])&&r.stopOnFalse&&(l=s.length,t=!1)}r.memory||(t=!1),i=!1,a&&(s=t?[]:"")},f={add:function(){return s&&(t&&!i&&(l=s.length-1,u.push(t)),function n(e){S.each(e,function(e,t){m(t)?r.unique&&f.has(t)||s.push(t):t&&t.length&&"string"!==w(t)&&n(t)})}(arguments),t&&!i&&c()),this},remove:function(){return S.each(arguments,function(e,t){var n;while(-1<(n=S.inArray(t,s,n)))s.splice(n,1),n<=l&&l--}),this},has:function(e){return e?-1<S.inArray(e,s):0<s.length},empty:function(){return s&&(s=[]),this},disable:function(){return a=u=[],s=t="",this},disabled:function(){return!s},lock:function(){return a=u=[],t||i||(s=t=""),this},locked:function(){return!!a},fireWith:function(e,t){return a||(t=[e,(t=t||[]).slice?t.slice():t],u.push(t),i||c()),this},fire:function(){return f.fireWith(this,arguments),this},fired:function(){return!!o}};return f},S.extend({Deferred:function(e){var o=[["notify","progress",S.Callbacks("memory"),S.Callbacks("memory"),2],["resolve","done",S.Callbacks("once memory"),S.Callbacks("once memory"),0,"resolved"],["reject","fail",S.Callbacks("once memory"),S.Callbacks("once memory"),1,"rejected"]],i="pending",a={state:function(){return i},always:function(){return s.done(arguments).fail(arguments),this},"catch":function(e){return a.then(null,e)},pipe:function(){var i=arguments;return S.Deferred(function(r){S.each(o,function(e,t){var n=m(i[t[4]])&&i[t[4]];s[t[1]](function(){var e=n&&n.apply(this,arguments);e&&m(e.promise)?e.promise().progress(r.notify).done(r.resolve).fail(r.reject):r[t[0]+"With"](this,n?[e]:arguments)})}),i=null}).promise()},then:function(t,n,r){var u=0;function l(i,o,a,s){return function(){var n=this,r=arguments,e=function(){var e,t;if(!(i<u)){if((e=a.apply(n,r))===o.promise())throw new TypeError("Thenable self-resolution");t=e&&("object"==typeof e||"function"==typeof e)&&e.then,m(t)?s?t.call(e,l(u,o,R,s),l(u,o,M,s)):(u++,t.call(e,l(u,o,R,s),l(u,o,M,s),l(u,o,R,o.notifyWith))):(a!==R&&(n=void 0,r=[e]),(s||o.resolveWith)(n,r))}},t=s?e:function(){try{e()}catch(e){S.Deferred.exceptionHook&&S.Deferred.exceptionHook(e,t.stackTrace),u<=i+1&&(a!==M&&(n=void 0,r=[e]),o.rejectWith(n,r))}};i?t():(S.Deferred.getStackHook&&(t.stackTrace=S.Deferred.getStackHook()),C.setTimeout(t))}}return S.Deferred(function(e){o[0][3].add(l(0,e,m(r)?r:R,e.notifyWith)),o[1][3].add(l(0,e,m(t)?t:R)),o[2][3].add(l(0,e,m(n)?n:M))}).promise()},promise:function(e){return null!=e?S.extend(e,a):a}},s={};return S.each(o,function(e,t){var n=t[2],r=t[5];a[t[1]]=n.add,r&&n.add(function(){i=r},o[3-e][2].disable,o[3-e][3].disable,o[0][2].lock,o[0][3].lock),n.add(t[3].fire),s[t[0]]=function(){return s[t[0]+"With"](this===s?void 0:this,arguments),this},s[t[0]+"With"]=n.fireWith}),a.promise(s),e&&e.call(s,s),s},when:function(e){var n=arguments.length,t=n,r=Array(t),i=s.call(arguments),o=S.Deferred(),a=function(t){return function(e){r[t]=this,i[t]=1<arguments.length?s.call(arguments):e,--n||o.resolveWith(r,i)}};if(n<=1&&(I(e,o.done(a(t)).resolve,o.reject,!n),"pending"===o.state()||m(i[t]&&i[t].then)))return o.then();while(t--)I(i[t],a(t),o.reject);return o.promise()}});var W=/^(Eval|Internal|Range|Reference|Syntax|Type|URI)Error$/;S.Deferred.exceptionHook=function(e,t){C.console&&C.console.warn&&e&&W.test(e.name)&&C.console.warn("jQuery.Deferred exception: "+e.message,e.stack,t)},S.readyException=function(e){C.setTimeout(function(){throw e})};var F=S.Deferred();function B(){E.removeEventListener("DOMContentLoaded",B),C.removeEventListener("load",B),S.ready()}S.fn.ready=function(e){return F.then(e)["catch"](function(e){S.readyException(e)}),this},S.extend({isReady:!1,readyWait:1,ready:function(e){(!0===e?--S.readyWait:S.isReady)||(S.isReady=!0)!==e&&0<--S.readyWait||F.resolveWith(E,[S])}}),S.ready.then=F.then,"complete"===E.readyState||"loading"!==E.readyState&&!E.documentElement.doScroll?C.setTimeout(S.ready):(E.addEventListener("DOMContentLoaded",B),C.addEventListener("load",B));var $=function(e,t,n,r,i,o,a){var s=0,u=e.length,l=null==n;if("object"===w(n))for(s in i=!0,n)$(e,t,s,n[s],!0,o,a);else if(void 0!==r&&(i=!0,m(r)||(a=!0),l&&(a?(t.call(e,r),t=null):(l=t,t=function(e,t,n){return l.call(S(e),n)})),t))for(;s<u;s++)t(e[s],n,a?r:r.call(e[s],s,t(e[s],n)));return i?e:l?t.call(e):u?t(e[0],n):o},_=/^-ms-/,z=/-([a-z])/g;function U(e,t){return t.toUpperCase()}function X(e){return e.replace(_,"ms-").replace(z,U)}var V=function(e){return 1===e.nodeType||9===e.nodeType||!+e.nodeType};function G(){this.expando=S.expando+G.uid++}G.uid=1,G.prototype={cache:function(e){var t=e[this.expando];return t||(t={},V(e)&&(e.nodeType?e[this.expando]=t:Object.defineProperty(e,this.expando,{value:t,configurable:!0}))),t},set:function(e,t,n){var r,i=this.cache(e);if("string"==typeof t)i[X(t)]=n;else for(r in t)i[X(r)]=t[r];return i},get:function(e,t){return void 0===t?this.cache(e):e[this.expando]&&e[this.expando][X(t)]},access:function(e,t,n){return void 0===t||t&&"string"==typeof t&&void 0===n?this.get(e,t):(this.set(e,t,n),void 0!==n?n:t)},remove:function(e,t){var n,r=e[this.expando];if(void 0!==r){if(void 0!==t){n=(t=Array.isArray(t)?t.map(X):(t=X(t))in r?[t]:t.match(P)||[]).length;while(n--)delete r[t[n]]}(void 0===t||S.isEmptyObject(r))&&(e.nodeType?e[this.expando]=void 0:delete e[this.expando])}},hasData:function(e){var t=e[this.expando];return void 0!==t&&!S.isEmptyObject(t)}};var Y=new G,Q=new G,J=/^(?:\{[\w\W]*\}|\[[\w\W]*\])$/,K=/[A-Z]/g;function Z(e,t,n){var r,i;if(void 0===n&&1===e.nodeType)if(r="data-"+t.replace(K,"-$&").toLowerCase(),"string"==typeof(n=e.getAttribute(r))){try{n="true"===(i=n)||"false"!==i&&("null"===i?null:i===+i+""?+i:J.test(i)?JSON.parse(i):i)}catch(e){}Q.set(e,t,n)}else n=void 0;return n}S.extend({hasData:function(e){return Q.hasData(e)||Y.hasData(e)},data:function(e,t,n){return Q.access(e,t,n)},removeData:function(e,t){Q.remove(e,t)},_data:function(e,t,n){return Y.access(e,t,n)},_removeData:function(e,t){Y.remove(e,t)}}),S.fn.extend({data:function(n,e){var t,r,i,o=this[0],a=o&&o.attributes;if(void 0===n){if(this.length&&(i=Q.get(o),1===o.nodeType&&!Y.get(o,"hasDataAttrs"))){t=a.length;while(t--)a[t]&&0===(r=a[t].name).indexOf("data-")&&(r=X(r.slice(5)),Z(o,r,i[r]));Y.set(o,"hasDataAttrs",!0)}return i}return"object"==typeof n?this.each(function(){Q.set(this,n)}):$(this,function(e){var t;if(o&&void 0===e)return void 0!==(t=Q.get(o,n))?t:void 0!==(t=Z(o,n))?t:void 0;this.each(function(){Q.set(this,n,e)})},null,e,1<arguments.length,null,!0)},removeData:function(e){return this.each(function(){Q.remove(this,e)})}}),S.extend({queue:function(e,t,n){var r;if(e)return t=(t||"fx")+"queue",r=Y.get(e,t),n&&(!r||Array.isArray(n)?r=Y.access(e,t,S.makeArray(n)):r.push(n)),r||[]},dequeue:function(e,t){t=t||"fx";var n=S.queue(e,t),r=n.length,i=n.shift(),o=S._queueHooks(e,t);"inprogress"===i&&(i=n.shift(),r--),i&&("fx"===t&&n.unshift("inprogress"),delete o.stop,i.call(e,function(){S.dequeue(e,t)},o)),!r&&o&&o.empty.fire()},_queueHooks:function(e,t){var n=t+"queueHooks";return Y.get(e,n)||Y.access(e,n,{empty:S.Callbacks("once memory").add(function(){Y.remove(e,[t+"queue",n])})})}}),S.fn.extend({queue:function(t,n){var e=2;return"string"!=typeof t&&(n=t,t="fx",e--),arguments.length<e?S.queue(this[0],t):void 0===n?this:this.each(function(){var e=S.queue(this,t,n);S._queueHooks(this,t),"fx"===t&&"inprogress"!==e[0]&&S.dequeue(this,t)})},dequeue:function(e){return this.each(function(){S.dequeue(this,e)})},clearQueue:function(e){return this.queue(e||"fx",[])},promise:function(e,t){var n,r=1,i=S.Deferred(),o=this,a=this.length,s=function(){--r||i.resolveWith(o,[o])};"string"!=typeof e&&(t=e,e=void 0),e=e||"fx";while(a--)(n=Y.get(o[a],e+"queueHooks"))&&n.empty&&(r++,n.empty.add(s));return s(),i.promise(t)}});var ee=/[+-]?(?:\d*\.|)\d+(?:[eE][+-]?\d+|)/.source,te=new RegExp("^(?:([+-])=|)("+ee+")([a-z%]*)$","i"),ne=["Top","Right","Bottom","Left"],re=E.documentElement,ie=function(e){return S.contains(e.ownerDocument,e)},oe={composed:!0};re.getRootNode&&(ie=function(e){return S.contains(e.ownerDocument,e)||e.getRootNode(oe)===e.ownerDocument});var ae=function(e,t){return"none"===(e=t||e).style.display||""===e.style.display&&ie(e)&&"none"===S.css(e,"display")};function se(e,t,n,r){var i,o,a=20,s=r?function(){return r.cur()}:function(){return S.css(e,t,"")},u=s(),l=n&&n[3]||(S.cssNumber[t]?"":"px"),c=e.nodeType&&(S.cssNumber[t]||"px"!==l&&+u)&&te.exec(S.css(e,t));if(c&&c[3]!==l){u/=2,l=l||c[3],c=+u||1;while(a--)S.style(e,t,c+l),(1-o)*(1-(o=s()/u||.5))<=0&&(a=0),c/=o;c*=2,S.style(e,t,c+l),n=n||[]}return n&&(c=+c||+u||0,i=n[1]?c+(n[1]+1)*n[2]:+n[2],r&&(r.unit=l,r.start=c,r.end=i)),i}var ue={};function le(e,t){for(var n,r,i,o,a,s,u,l=[],c=0,f=e.length;c<f;c++)(r=e[c]).style&&(n=r.style.display,t?("none"===n&&(l[c]=Y.get(r,"display")||null,l[c]||(r.style.display="")),""===r.style.display&&ae(r)&&(l[c]=(u=a=o=void 0,a=(i=r).ownerDocument,s=i.nodeName,(u=ue[s])||(o=a.body.appendChild(a.createElement(s)),u=S.css(o,"display"),o.parentNode.removeChild(o),"none"===u&&(u="block"),ue[s]=u)))):"none"!==n&&(l[c]="none",Y.set(r,"display",n)));for(c=0;c<f;c++)null!=l[c]&&(e[c].style.display=l[c]);return e}S.fn.extend({show:function(){return le(this,!0)},hide:function(){return le(this)},toggle:function(e){return"boolean"==typeof e?e?this.show():this.hide():this.each(function(){ae(this)?S(this).show():S(this).hide()})}});var ce,fe,pe=/^(?:checkbox|radio)$/i,de=/<([a-z][^\/\0>\x20\t\r\n\f]*)/i,he=/^$|^module$|\/(?:java|ecma)script/i;ce=E.createDocumentFragment().appendChild(E.createElement("div")),(fe=E.createElement("input")).setAttribute("type","radio"),fe.setAttribute("checked","checked"),fe.setAttribute("name","t"),ce.appendChild(fe),y.checkClone=ce.cloneNode(!0).cloneNode(!0).lastChild.checked,ce.innerHTML="<textarea>x</textarea>",y.noCloneChecked=!!ce.cloneNode(!0).lastChild.defaultValue,ce.innerHTML="<option></option>",y.option=!!ce.lastChild;var ge={thead:[1,"<table>","</table>"],col:[2,"<table><colgroup>","</colgroup></table>"],tr:[2,"<table><tbody>","</tbody></table>"],td:[3,"<table><tbody><tr>","</tr></tbody></table>"],_default:[0,"",""]};function ve(e,t){var n;return n="undefined"!=typeof e.getElementsByTagName?e.getElementsByTagName(t||"*"):"undefined"!=typeof e.querySelectorAll?e.querySelectorAll(t||"*"):[],void 0===t||t&&A(e,t)?S.merge([e],n):n}function ye(e,t){for(var n=0,r=e.length;n<r;n++)Y.set(e[n],"globalEval",!t||Y.get(t[n],"globalEval"))}ge.tbody=ge.tfoot=ge.colgroup=ge.caption=ge.thead,ge.th=ge.td,y.option||(ge.optgroup=ge.option=[1,"<select multiple='multiple'>","</select>"]);var me=/<|&#?\w+;/;function xe(e,t,n,r,i){for(var o,a,s,u,l,c,f=t.createDocumentFragment(),p=[],d=0,h=e.length;d<h;d++)if((o=e[d])||0===o)if("object"===w(o))S.merge(p,o.nodeType?[o]:o);else if(me.test(o)){a=a||f.appendChild(t.createElement("div")),s=(de.exec(o)||["",""])[1].toLowerCase(),u=ge[s]||ge._default,a.innerHTML=u[1]+S.htmlPrefilter(o)+u[2],c=u[0];while(c--)a=a.lastChild;S.merge(p,a.childNodes),(a=f.firstChild).textContent=""}else p.push(t.createTextNode(o));f.textContent="",d=0;while(o=p[d++])if(r&&-1<S.inArray(o,r))i&&i.push(o);else if(l=ie(o),a=ve(f.appendChild(o),"script"),l&&ye(a),n){c=0;while(o=a[c++])he.test(o.type||"")&&n.push(o)}return f}var be=/^key/,we=/^(?:mouse|pointer|contextmenu|drag|drop)|click/,Te=/^([^.]*)(?:\.(.+)|)/;function Ce(){return!0}function Ee(){return!1}function Se(e,t){return e===function(){try{return E.activeElement}catch(e){}}()==("focus"===t)}function ke(e,t,n,r,i,o){var a,s;if("object"==typeof t){for(s in"string"!=typeof n&&(r=r||n,n=void 0),t)ke(e,s,n,r,t[s],o);return e}if(null==r&&null==i?(i=n,r=n=void 0):null==i&&("string"==typeof n?(i=r,r=void 0):(i=r,r=n,n=void 0)),!1===i)i=Ee;else if(!i)return e;return 1===o&&(a=i,(i=function(e){return S().off(e),a.apply(this,arguments)}).guid=a.guid||(a.guid=S.guid++)),e.each(function(){S.event.add(this,t,i,r,n)})}function Ae(e,i,o){o?(Y.set(e,i,!1),S.event.add(e,i,{namespace:!1,handler:function(e){var t,n,r=Y.get(this,i);if(1&e.isTrigger&&this[i]){if(r.length)(S.event.special[i]||{}).delegateType&&e.stopPropagation();else if(r=s.call(arguments),Y.set(this,i,r),t=o(this,i),this[i](),r!==(n=Y.get(this,i))||t?Y.set(this,i,!1):n={},r!==n)return e.stopImmediatePropagation(),e.preventDefault(),n.value}else r.length&&(Y.set(this,i,{value:S.event.trigger(S.extend(r[0],S.Event.prototype),r.slice(1),this)}),e.stopImmediatePropagation())}})):void 0===Y.get(e,i)&&S.event.add(e,i,Ce)}S.event={global:{},add:function(t,e,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,v=Y.get(t);if(V(t)){n.handler&&(n=(o=n).handler,i=o.selector),i&&S.find.matchesSelector(re,i),n.guid||(n.guid=S.guid++),(u=v.events)||(u=v.events=Object.create(null)),(a=v.handle)||(a=v.handle=function(e){return"undefined"!=typeof S&&S.event.triggered!==e.type?S.event.dispatch.apply(t,arguments):void 0}),l=(e=(e||"").match(P)||[""]).length;while(l--)d=g=(s=Te.exec(e[l])||[])[1],h=(s[2]||"").split(".").sort(),d&&(f=S.event.special[d]||{},d=(i?f.delegateType:f.bindType)||d,f=S.event.special[d]||{},c=S.extend({type:d,origType:g,data:r,handler:n,guid:n.guid,selector:i,needsContext:i&&S.expr.match.needsContext.test(i),namespace:h.join(".")},o),(p=u[d])||((p=u[d]=[]).delegateCount=0,f.setup&&!1!==f.setup.call(t,r,h,a)||t.addEventListener&&t.addEventListener(d,a)),f.add&&(f.add.call(t,c),c.handler.guid||(c.handler.guid=n.guid)),i?p.splice(p.delegateCount++,0,c):p.push(c),S.event.global[d]=!0)}},remove:function(e,t,n,r,i){var o,a,s,u,l,c,f,p,d,h,g,v=Y.hasData(e)&&Y.get(e);if(v&&(u=v.events)){l=(t=(t||"").match(P)||[""]).length;while(l--)if(d=g=(s=Te.exec(t[l])||[])[1],h=(s[2]||"").split(".").sort(),d){f=S.event.special[d]||{},p=u[d=(r?f.delegateType:f.bindType)||d]||[],s=s[2]&&new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"),a=o=p.length;while(o--)c=p[o],!i&&g!==c.origType||n&&n.guid!==c.guid||s&&!s.test(c.namespace)||r&&r!==c.selector&&("**"!==r||!c.selector)||(p.splice(o,1),c.selector&&p.delegateCount--,f.remove&&f.remove.call(e,c));a&&!p.length&&(f.teardown&&!1!==f.teardown.call(e,h,v.handle)||S.removeEvent(e,d,v.handle),delete u[d])}else for(d in u)S.event.remove(e,d+t[l],n,r,!0);S.isEmptyObject(u)&&Y.remove(e,"handle events")}},dispatch:function(e){var t,n,r,i,o,a,s=new Array(arguments.length),u=S.event.fix(e),l=(Y.get(this,"events")||Object.create(null))[u.type]||[],c=S.event.special[u.type]||{};for(s[0]=u,t=1;t<arguments.length;t++)s[t]=arguments[t];if(u.delegateTarget=this,!c.preDispatch||!1!==c.preDispatch.call(this,u)){a=S.event.handlers.call(this,u,l),t=0;while((i=a[t++])&&!u.isPropagationStopped()){u.currentTarget=i.elem,n=0;while((o=i.handlers[n++])&&!u.isImmediatePropagationStopped())u.rnamespace&&!1!==o.namespace&&!u.rnamespace.test(o.namespace)||(u.handleObj=o,u.data=o.data,void 0!==(r=((S.event.special[o.origType]||{}).handle||o.handler).apply(i.elem,s))&&!1===(u.result=r)&&(u.preventDefault(),u.stopPropagation()))}return c.postDispatch&&c.postDispatch.call(this,u),u.result}},handlers:function(e,t){var n,r,i,o,a,s=[],u=t.delegateCount,l=e.target;if(u&&l.nodeType&&!("click"===e.type&&1<=e.button))for(;l!==this;l=l.parentNode||this)if(1===l.nodeType&&("click"!==e.type||!0!==l.disabled)){for(o=[],a={},n=0;n<u;n++)void 0===a[i=(r=t[n]).selector+" "]&&(a[i]=r.needsContext?-1<S(i,this).index(l):S.find(i,this,null,[l]).length),a[i]&&o.push(r);o.length&&s.push({elem:l,handlers:o})}return l=this,u<t.length&&s.push({elem:l,handlers:t.slice(u)}),s},addProp:function(t,e){Object.defineProperty(S.Event.prototype,t,{enumerable:!0,configurable:!0,get:m(e)?function(){if(this.originalEvent)return e(this.originalEvent)}:function(){if(this.originalEvent)return this.originalEvent[t]},set:function(e){Object.defineProperty(this,t,{enumerable:!0,configurable:!0,writable:!0,value:e})}})},fix:function(e){return e[S.expando]?e:new S.Event(e)},special:{load:{noBubble:!0},click:{setup:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Ae(t,"click",Ce),!1},trigger:function(e){var t=this||e;return pe.test(t.type)&&t.click&&A(t,"input")&&Ae(t,"click"),!0},_default:function(e){var t=e.target;return pe.test(t.type)&&t.click&&A(t,"input")&&Y.get(t,"click")||A(t,"a")}},beforeunload:{postDispatch:function(e){void 0!==e.result&&e.originalEvent&&(e.originalEvent.returnValue=e.result)}}}},S.removeEvent=function(e,t,n){e.removeEventListener&&e.removeEventListener(t,n)},S.Event=function(e,t){if(!(this instanceof S.Event))return new S.Event(e,t);e&&e.type?(this.originalEvent=e,this.type=e.type,this.isDefaultPrevented=e.defaultPrevented||void 0===e.defaultPrevented&&!1===e.returnValue?Ce:Ee,this.target=e.target&&3===e.target.nodeType?e.target.parentNode:e.target,this.currentTarget=e.currentTarget,this.relatedTarget=e.relatedTarget):this.type=e,t&&S.extend(this,t),this.timeStamp=e&&e.timeStamp||Date.now(),this[S.expando]=!0},S.Event.prototype={constructor:S.Event,isDefaultPrevented:Ee,isPropagationStopped:Ee,isImmediatePropagationStopped:Ee,isSimulated:!1,preventDefault:function(){var e=this.originalEvent;this.isDefaultPrevented=Ce,e&&!this.isSimulated&&e.preventDefault()},stopPropagation:function(){var e=this.originalEvent;this.isPropagationStopped=Ce,e&&!this.isSimulated&&e.stopPropagation()},stopImmediatePropagation:function(){var e=this.originalEvent;this.isImmediatePropagationStopped=Ce,e&&!this.isSimulated&&e.stopImmediatePropagation(),this.stopPropagation()}},S.each({altKey:!0,bubbles:!0,cancelable:!0,changedTouches:!0,ctrlKey:!0,detail:!0,eventPhase:!0,metaKey:!0,pageX:!0,pageY:!0,shiftKey:!0,view:!0,"char":!0,code:!0,charCode:!0,key:!0,keyCode:!0,button:!0,buttons:!0,clientX:!0,clientY:!0,offsetX:!0,offsetY:!0,pointerId:!0,pointerType:!0,screenX:!0,screenY:!0,targetTouches:!0,toElement:!0,touches:!0,which:function(e){var t=e.button;return null==e.which&&be.test(e.type)?null!=e.charCode?e.charCode:e.keyCode:!e.which&&void 0!==t&&we.test(e.type)?1&t?1:2&t?3:4&t?2:0:e.which}},S.event.addProp),S.each({focus:"focusin",blur:"focusout"},function(e,t){S.event.special[e]={setup:function(){return Ae(this,e,Se),!1},trigger:function(){return Ae(this,e),!0},delegateType:t}}),S.each({mouseenter:"mouseover",mouseleave:"mouseout",pointerenter:"pointerover",pointerleave:"pointerout"},function(e,i){S.event.special[e]={delegateType:i,bindType:i,handle:function(e){var t,n=e.relatedTarget,r=e.handleObj;return n&&(n===this||S.contains(this,n))||(e.type=r.origType,t=r.handler.apply(this,arguments),e.type=i),t}}}),S.fn.extend({on:function(e,t,n,r){return ke(this,e,t,n,r)},one:function(e,t,n,r){return ke(this,e,t,n,r,1)},off:function(e,t,n){var r,i;if(e&&e.preventDefault&&e.handleObj)return r=e.handleObj,S(e.delegateTarget).off(r.namespace?r.origType+"."+r.namespace:r.origType,r.selector,r.handler),this;if("object"==typeof e){for(i in e)this.off(i,t,e[i]);return this}return!1!==t&&"function"!=typeof t||(n=t,t=void 0),!1===n&&(n=Ee),this.each(function(){S.event.remove(this,e,n,t)})}});var Ne=/<script|<style|<link/i,De=/checked\s*(?:[^=]|=\s*.checked.)/i,je=/^\s*<!(?:\[CDATA\[|--)|(?:\]\]|--)>\s*$/g;function qe(e,t){return A(e,"table")&&A(11!==t.nodeType?t:t.firstChild,"tr")&&S(e).children("tbody")[0]||e}function Le(e){return e.type=(null!==e.getAttribute("type"))+"/"+e.type,e}function He(e){return"true/"===(e.type||"").slice(0,5)?e.type=e.type.slice(5):e.removeAttribute("type"),e}function Oe(e,t){var n,r,i,o,a,s;if(1===t.nodeType){if(Y.hasData(e)&&(s=Y.get(e).events))for(i in Y.remove(t,"handle events"),s)for(n=0,r=s[i].length;n<r;n++)S.event.add(t,i,s[i][n]);Q.hasData(e)&&(o=Q.access(e),a=S.extend({},o),Q.set(t,a))}}function Pe(n,r,i,o){r=g(r);var e,t,a,s,u,l,c=0,f=n.length,p=f-1,d=r[0],h=m(d);if(h||1<f&&"string"==typeof d&&!y.checkClone&&De.test(d))return n.each(function(e){var t=n.eq(e);h&&(r[0]=d.call(this,e,t.html())),Pe(t,r,i,o)});if(f&&(t=(e=xe(r,n[0].ownerDocument,!1,n,o)).firstChild,1===e.childNodes.length&&(e=t),t||o)){for(s=(a=S.map(ve(e,"script"),Le)).length;c<f;c++)u=e,c!==p&&(u=S.clone(u,!0,!0),s&&S.merge(a,ve(u,"script"))),i.call(n[c],u,c);if(s)for(l=a[a.length-1].ownerDocument,S.map(a,He),c=0;c<s;c++)u=a[c],he.test(u.type||"")&&!Y.access(u,"globalEval")&&S.contains(l,u)&&(u.src&&"module"!==(u.type||"").toLowerCase()?S._evalUrl&&!u.noModule&&S._evalUrl(u.src,{nonce:u.nonce||u.getAttribute("nonce")},l):b(u.textContent.replace(je,""),u,l))}return n}function Re(e,t,n){for(var r,i=t?S.filter(t,e):e,o=0;null!=(r=i[o]);o++)n||1!==r.nodeType||S.cleanData(ve(r)),r.parentNode&&(n&&ie(r)&&ye(ve(r,"script")),r.parentNode.removeChild(r));return e}S.extend({htmlPrefilter:function(e){return e},clone:function(e,t,n){var r,i,o,a,s,u,l,c=e.cloneNode(!0),f=ie(e);if(!(y.noCloneChecked||1!==e.nodeType&&11!==e.nodeType||S.isXMLDoc(e)))for(a=ve(c),r=0,i=(o=ve(e)).length;r<i;r++)s=o[r],u=a[r],void 0,"input"===(l=u.nodeName.toLowerCase())&&pe.test(s.type)?u.checked=s.checked:"input"!==l&&"textarea"!==l||(u.defaultValue=s.defaultValue);if(t)if(n)for(o=o||ve(e),a=a||ve(c),r=0,i=o.length;r<i;r++)Oe(o[r],a[r]);else Oe(e,c);return 0<(a=ve(c,"script")).length&&ye(a,!f&&ve(e,"script")),c},cleanData:function(e){for(var t,n,r,i=S.event.special,o=0;void 0!==(n=e[o]);o++)if(V(n)){if(t=n[Y.expando]){if(t.events)for(r in t.events)i[r]?S.event.remove(n,r):S.removeEvent(n,r,t.handle);n[Y.expando]=void 0}n[Q.expando]&&(n[Q.expando]=void 0)}}}),S.fn.extend({detach:function(e){return Re(this,e,!0)},remove:function(e){return Re(this,e)},text:function(e){return $(this,function(e){return void 0===e?S.text(this):this.empty().each(function(){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||(this.textContent=e)})},null,e,arguments.length)},append:function(){return Pe(this,arguments,function(e){1!==this.nodeType&&11!==this.nodeType&&9!==this.nodeType||qe(this,e).appendChild(e)})},prepend:function(){return Pe(this,arguments,function(e){if(1===this.nodeType||11===this.nodeType||9===this.nodeType){var t=qe(this,e);t.insertBefore(e,t.firstChild)}})},before:function(){return Pe(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this)})},after:function(){return Pe(this,arguments,function(e){this.parentNode&&this.parentNode.insertBefore(e,this.nextSibling)})},empty:function(){for(var e,t=0;null!=(e=this[t]);t++)1===e.nodeType&&(S.cleanData(ve(e,!1)),e.textContent="");return this},clone:function(e,t){return e=null!=e&&e,t=null==t?e:t,this.map(function(){return S.clone(this,e,t)})},html:function(e){return $(this,function(e){var t=this[0]||{},n=0,r=this.length;if(void 0===e&&1===t.nodeType)return t.innerHTML;if("string"==typeof e&&!Ne.test(e)&&!ge[(de.exec(e)||["",""])[1].toLowerCase()]){e=S.htmlPrefilter(e);try{for(;n<r;n++)1===(t=this[n]||{}).nodeType&&(S.cleanData(ve(t,!1)),t.innerHTML=e);t=0}catch(e){}}t&&this.empty().append(e)},null,e,arguments.length)},replaceWith:function(){var n=[];return Pe(this,arguments,function(e){var t=this.parentNode;S.inArray(this,n)<0&&(S.cleanData(ve(this)),t&&t.replaceChild(e,this))},n)}}),S.each({appendTo:"append",prependTo:"prepend",insertBefore:"before",insertAfter:"after",replaceAll:"replaceWith"},function(e,a){S.fn[e]=function(e){for(var t,n=[],r=S(e),i=r.length-1,o=0;o<=i;o++)t=o===i?this:this.clone(!0),S(r[o])[a](t),u.apply(n,t.get());return this.pushStack(n)}});var Me=new RegExp("^("+ee+")(?!px)[a-z%]+$","i"),Ie=function(e){var t=e.ownerDocument.defaultView;return t&&t.opener||(t=C),t.getComputedStyle(e)},We=function(e,t,n){var r,i,o={};for(i in t)o[i]=e.style[i],e.style[i]=t[i];for(i in r=n.call(e),t)e.style[i]=o[i];return r},Fe=new RegExp(ne.join("|"),"i");function Be(e,t,n){var r,i,o,a,s=e.style;return(n=n||Ie(e))&&(""!==(a=n.getPropertyValue(t)||n[t])||ie(e)||(a=S.style(e,t)),!y.pixelBoxStyles()&&Me.test(a)&&Fe.test(t)&&(r=s.width,i=s.minWidth,o=s.maxWidth,s.minWidth=s.maxWidth=s.width=a,a=n.width,s.width=r,s.minWidth=i,s.maxWidth=o)),void 0!==a?a+"":a}function $e(e,t){return{get:function(){if(!e())return(this.get=t).apply(this,arguments);delete this.get}}}!function(){function e(){if(l){u.style.cssText="position:absolute;left:-11111px;width:60px;margin-top:1px;padding:0;border:0",l.style.cssText="position:relative;display:block;box-sizing:border-box;overflow:scroll;margin:auto;border:1px;padding:1px;width:60%;top:1%",re.appendChild(u).appendChild(l);var e=C.getComputedStyle(l);n="1%"!==e.top,s=12===t(e.marginLeft),l.style.right="60%",o=36===t(e.right),r=36===t(e.width),l.style.position="absolute",i=12===t(l.offsetWidth/3),re.removeChild(u),l=null}}function t(e){return Math.round(parseFloat(e))}var n,r,i,o,a,s,u=E.createElement("div"),l=E.createElement("div");l.style&&(l.style.backgroundClip="content-box",l.cloneNode(!0).style.backgroundClip="",y.clearCloneStyle="content-box"===l.style.backgroundClip,S.extend(y,{boxSizingReliable:function(){return e(),r},pixelBoxStyles:function(){return e(),o},pixelPosition:function(){return e(),n},reliableMarginLeft:function(){return e(),s},scrollboxSize:function(){return e(),i},reliableTrDimensions:function(){var e,t,n,r;return null==a&&(e=E.createElement("table"),t=E.createElement("tr"),n=E.createElement("div"),e.style.cssText="position:absolute;left:-11111px",t.style.height="1px",n.style.height="9px",re.appendChild(e).appendChild(t).appendChild(n),r=C.getComputedStyle(t),a=3<parseInt(r.height),re.removeChild(e)),a}}))}();var _e=["Webkit","Moz","ms"],ze=E.createElement("div").style,Ue={};function Xe(e){var t=S.cssProps[e]||Ue[e];return t||(e in ze?e:Ue[e]=function(e){var t=e[0].toUpperCase()+e.slice(1),n=_e.length;while(n--)if((e=_e[n]+t)in ze)return e}(e)||e)}var Ve=/^(none|table(?!-c[ea]).+)/,Ge=/^--/,Ye={position:"absolute",visibility:"hidden",display:"block"},Qe={letterSpacing:"0",fontWeight:"400"};function Je(e,t,n){var r=te.exec(t);return r?Math.max(0,r[2]-(n||0))+(r[3]||"px"):t}function Ke(e,t,n,r,i,o){var a="width"===t?1:0,s=0,u=0;if(n===(r?"border":"content"))return 0;for(;a<4;a+=2)"margin"===n&&(u+=S.css(e,n+ne[a],!0,i)),r?("content"===n&&(u-=S.css(e,"padding"+ne[a],!0,i)),"margin"!==n&&(u-=S.css(e,"border"+ne[a]+"Width",!0,i))):(u+=S.css(e,"padding"+ne[a],!0,i),"padding"!==n?u+=S.css(e,"border"+ne[a]+"Width",!0,i):s+=S.css(e,"border"+ne[a]+"Width",!0,i));return!r&&0<=o&&(u+=Math.max(0,Math.ceil(e["offset"+t[0].toUpperCase()+t.slice(1)]-o-u-s-.5))||0),u}function Ze(e,t,n){var r=Ie(e),i=(!y.boxSizingReliable()||n)&&"border-box"===S.css(e,"boxSizing",!1,r),o=i,a=Be(e,t,r),s="offset"+t[0].toUpperCase()+t.slice(1);if(Me.test(a)){if(!n)return a;a="auto"}return(!y.boxSizingReliable()&&i||!y.reliableTrDimensions()&&A(e,"tr")||"auto"===a||!parseFloat(a)&&"inline"===S.css(e,"display",!1,r))&&e.getClientRects().length&&(i="border-box"===S.css(e,"boxSizing",!1,r),(o=s in e)&&(a=e[s])),(a=parseFloat(a)||0)+Ke(e,t,n||(i?"border":"content"),o,r,a)+"px"}function et(e,t,n,r,i){return new et.prototype.init(e,t,n,r,i)}S.extend({cssHooks:{opacity:{get:function(e,t){if(t){var n=Be(e,"opacity");return""===n?"1":n}}}},cssNumber:{animationIterationCount:!0,columnCount:!0,fillOpacity:!0,flexGrow:!0,flexShrink:!0,fontWeight:!0,gridArea:!0,gridColumn:!0,gridColumnEnd:!0,gridColumnStart:!0,gridRow:!0,gridRowEnd:!0,gridRowStart:!0,lineHeight:!0,opacity:!0,order:!0,orphans:!0,widows:!0,zIndex:!0,zoom:!0},cssProps:{},style:function(e,t,n,r){if(e&&3!==e.nodeType&&8!==e.nodeType&&e.style){var i,o,a,s=X(t),u=Ge.test(t),l=e.style;if(u||(t=Xe(s)),a=S.cssHooks[t]||S.cssHooks[s],void 0===n)return a&&"get"in a&&void 0!==(i=a.get(e,!1,r))?i:l[t];"string"===(o=typeof n)&&(i=te.exec(n))&&i[1]&&(n=se(e,t,i),o="number"),null!=n&&n==n&&("number"!==o||u||(n+=i&&i[3]||(S.cssNumber[s]?"":"px")),y.clearCloneStyle||""!==n||0!==t.indexOf("background")||(l[t]="inherit"),a&&"set"in a&&void 0===(n=a.set(e,n,r))||(u?l.setProperty(t,n):l[t]=n))}},css:function(e,t,n,r){var i,o,a,s=X(t);return Ge.test(t)||(t=Xe(s)),(a=S.cssHooks[t]||S.cssHooks[s])&&"get"in a&&(i=a.get(e,!0,n)),void 0===i&&(i=Be(e,t,r)),"normal"===i&&t in Qe&&(i=Qe[t]),""===n||n?(o=parseFloat(i),!0===n||isFinite(o)?o||0:i):i}}),S.each(["height","width"],function(e,u){S.cssHooks[u]={get:function(e,t,n){if(t)return!Ve.test(S.css(e,"display"))||e.getClientRects().length&&e.getBoundingClientRect().width?Ze(e,u,n):We(e,Ye,function(){return Ze(e,u,n)})},set:function(e,t,n){var r,i=Ie(e),o=!y.scrollboxSize()&&"absolute"===i.position,a=(o||n)&&"border-box"===S.css(e,"boxSizing",!1,i),s=n?Ke(e,u,n,a,i):0;return a&&o&&(s-=Math.ceil(e["offset"+u[0].toUpperCase()+u.slice(1)]-parseFloat(i[u])-Ke(e,u,"border",!1,i)-.5)),s&&(r=te.exec(t))&&"px"!==(r[3]||"px")&&(e.style[u]=t,t=S.css(e,u)),Je(0,t,s)}}}),S.cssHooks.marginLeft=$e(y.reliableMarginLeft,function(e,t){if(t)return(parseFloat(Be(e,"marginLeft"))||e.getBoundingClientRect().left-We(e,{marginLeft:0},function(){return e.getBoundingClientRect().left}))+"px"}),S.each({margin:"",padding:"",border:"Width"},function(i,o){S.cssHooks[i+o]={expand:function(e){for(var t=0,n={},r="string"==typeof e?e.split(" "):[e];t<4;t++)n[i+ne[t]+o]=r[t]||r[t-2]||r[0];return n}},"margin"!==i&&(S.cssHooks[i+o].set=Je)}),S.fn.extend({css:function(e,t){return $(this,function(e,t,n){var r,i,o={},a=0;if(Array.isArray(t)){for(r=Ie(e),i=t.length;a<i;a++)o[t[a]]=S.css(e,t[a],!1,r);return o}return void 0!==n?S.style(e,t,n):S.css(e,t)},e,t,1<arguments.length)}}),((S.Tween=et).prototype={constructor:et,init:function(e,t,n,r,i,o){this.elem=e,this.prop=n,this.easing=i||S.easing._default,this.options=t,this.start=this.now=this.cur(),this.end=r,this.unit=o||(S.cssNumber[n]?"":"px")},cur:function(){var e=et.propHooks[this.prop];return e&&e.get?e.get(this):et.propHooks._default.get(this)},run:function(e){var t,n=et.propHooks[this.prop];return this.options.duration?this.pos=t=S.easing[this.easing](e,this.options.duration*e,0,1,this.options.duration):this.pos=t=e,this.now=(this.end-this.start)*t+this.start,this.options.step&&this.options.step.call(this.elem,this.now,this),n&&n.set?n.set(this):et.propHooks._default.set(this),this}}).init.prototype=et.prototype,(et.propHooks={_default:{get:function(e){var t;return 1!==e.elem.nodeType||null!=e.elem[e.prop]&&null==e.elem.style[e.prop]?e.elem[e.prop]:(t=S.css(e.elem,e.prop,""))&&"auto"!==t?t:0},set:function(e){S.fx.step[e.prop]?S.fx.step[e.prop](e):1!==e.elem.nodeType||!S.cssHooks[e.prop]&&null==e.elem.style[Xe(e.prop)]?e.elem[e.prop]=e.now:S.style(e.elem,e.prop,e.now+e.unit)}}}).scrollTop=et.propHooks.scrollLeft={set:function(e){e.elem.nodeType&&e.elem.parentNode&&(e.elem[e.prop]=e.now)}},S.easing={linear:function(e){return e},swing:function(e){return.5-Math.cos(e*Math.PI)/2},_default:"swing"},S.fx=et.prototype.init,S.fx.step={};var tt,nt,rt,it,ot=/^(?:toggle|show|hide)$/,at=/queueHooks$/;function st(){nt&&(!1===E.hidden&&C.requestAnimationFrame?C.requestAnimationFrame(st):C.setTimeout(st,S.fx.interval),S.fx.tick())}function ut(){return C.setTimeout(function(){tt=void 0}),tt=Date.now()}function lt(e,t){var n,r=0,i={height:e};for(t=t?1:0;r<4;r+=2-t)i["margin"+(n=ne[r])]=i["padding"+n]=e;return t&&(i.opacity=i.width=e),i}function ct(e,t,n){for(var r,i=(ft.tweeners[t]||[]).concat(ft.tweeners["*"]),o=0,a=i.length;o<a;o++)if(r=i[o].call(n,t,e))return r}function ft(o,e,t){var n,a,r=0,i=ft.prefilters.length,s=S.Deferred().always(function(){delete u.elem}),u=function(){if(a)return!1;for(var e=tt||ut(),t=Math.max(0,l.startTime+l.duration-e),n=1-(t/l.duration||0),r=0,i=l.tweens.length;r<i;r++)l.tweens[r].run(n);return s.notifyWith(o,[l,n,t]),n<1&&i?t:(i||s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l]),!1)},l=s.promise({elem:o,props:S.extend({},e),opts:S.extend(!0,{specialEasing:{},easing:S.easing._default},t),originalProperties:e,originalOptions:t,startTime:tt||ut(),duration:t.duration,tweens:[],createTween:function(e,t){var n=S.Tween(o,l.opts,e,t,l.opts.specialEasing[e]||l.opts.easing);return l.tweens.push(n),n},stop:function(e){var t=0,n=e?l.tweens.length:0;if(a)return this;for(a=!0;t<n;t++)l.tweens[t].run(1);return e?(s.notifyWith(o,[l,1,0]),s.resolveWith(o,[l,e])):s.rejectWith(o,[l,e]),this}}),c=l.props;for(!function(e,t){var n,r,i,o,a;for(n in e)if(i=t[r=X(n)],o=e[n],Array.isArray(o)&&(i=o[1],o=e[n]=o[0]),n!==r&&(e[r]=o,delete e[n]),(a=S.cssHooks[r])&&"expand"in a)for(n in o=a.expand(o),delete e[r],o)n in e||(e[n]=o[n],t[n]=i);else t[r]=i}(c,l.opts.specialEasing);r<i;r++)if(n=ft.prefilters[r].call(l,o,c,l.opts))return m(n.stop)&&(S._queueHooks(l.elem,l.opts.queue).stop=n.stop.bind(n)),n;return S.map(c,ct,l),m(l.opts.start)&&l.opts.start.call(o,l),l.progress(l.opts.progress).done(l.opts.done,l.opts.complete).fail(l.opts.fail).always(l.opts.always),S.fx.timer(S.extend(u,{elem:o,anim:l,queue:l.opts.queue})),l}S.Animation=S.extend(ft,{tweeners:{"*":[function(e,t){var n=this.createTween(e,t);return se(n.elem,e,te.exec(t),n),n}]},tweener:function(e,t){m(e)?(t=e,e=["*"]):e=e.match(P);for(var n,r=0,i=e.length;r<i;r++)n=e[r],ft.tweeners[n]=ft.tweeners[n]||[],ft.tweeners[n].unshift(t)},prefilters:[function(e,t,n){var r,i,o,a,s,u,l,c,f="width"in t||"height"in t,p=this,d={},h=e.style,g=e.nodeType&&ae(e),v=Y.get(e,"fxshow");for(r in n.queue||(null==(a=S._queueHooks(e,"fx")).unqueued&&(a.unqueued=0,s=a.empty.fire,a.empty.fire=function(){a.unqueued||s()}),a.unqueued++,p.always(function(){p.always(function(){a.unqueued--,S.queue(e,"fx").length||a.empty.fire()})})),t)if(i=t[r],ot.test(i)){if(delete t[r],o=o||"toggle"===i,i===(g?"hide":"show")){if("show"!==i||!v||void 0===v[r])continue;g=!0}d[r]=v&&v[r]||S.style(e,r)}if((u=!S.isEmptyObject(t))||!S.isEmptyObject(d))for(r in f&&1===e.nodeType&&(n.overflow=[h.overflow,h.overflowX,h.overflowY],null==(l=v&&v.display)&&(l=Y.get(e,"display")),"none"===(c=S.css(e,"display"))&&(l?c=l:(le([e],!0),l=e.style.display||l,c=S.css(e,"display"),le([e]))),("inline"===c||"inline-block"===c&&null!=l)&&"none"===S.css(e,"float")&&(u||(p.done(function(){h.display=l}),null==l&&(c=h.display,l="none"===c?"":c)),h.display="inline-block")),n.overflow&&(h.overflow="hidden",p.always(function(){h.overflow=n.overflow[0],h.overflowX=n.overflow[1],h.overflowY=n.overflow[2]})),u=!1,d)u||(v?"hidden"in v&&(g=v.hidden):v=Y.access(e,"fxshow",{display:l}),o&&(v.hidden=!g),g&&le([e],!0),p.done(function(){for(r in g||le([e]),Y.remove(e,"fxshow"),d)S.style(e,r,d[r])})),u=ct(g?v[r]:0,r,p),r in v||(v[r]=u.start,g&&(u.end=u.start,u.start=0))}],prefilter:function(e,t){t?ft.prefilters.unshift(e):ft.prefilters.push(e)}}),S.speed=function(e,t,n){var r=e&&"object"==typeof e?S.extend({},e):{complete:n||!n&&t||m(e)&&e,duration:e,easing:n&&t||t&&!m(t)&&t};return S.fx.off?r.duration=0:"number"!=typeof r.duration&&(r.duration in S.fx.speeds?r.duration=S.fx.speeds[r.duration]:r.duration=S.fx.speeds._default),null!=r.queue&&!0!==r.queue||(r.queue="fx"),r.old=r.complete,r.complete=function(){m(r.old)&&r.old.call(this),r.queue&&S.dequeue(this,r.queue)},r},S.fn.extend({fadeTo:function(e,t,n,r){return this.filter(ae).css("opacity",0).show().end().animate({opacity:t},e,n,r)},animate:function(t,e,n,r){var i=S.isEmptyObject(t),o=S.speed(e,n,r),a=function(){var e=ft(this,S.extend({},t),o);(i||Y.get(this,"finish"))&&e.stop(!0)};return a.finish=a,i||!1===o.queue?this.each(a):this.queue(o.queue,a)},stop:function(i,e,o){var a=function(e){var t=e.stop;delete e.stop,t(o)};return"string"!=typeof i&&(o=e,e=i,i=void 0),e&&this.queue(i||"fx",[]),this.each(function(){var e=!0,t=null!=i&&i+"queueHooks",n=S.timers,r=Y.get(this);if(t)r[t]&&r[t].stop&&a(r[t]);else for(t in r)r[t]&&r[t].stop&&at.test(t)&&a(r[t]);for(t=n.length;t--;)n[t].elem!==this||null!=i&&n[t].queue!==i||(n[t].anim.stop(o),e=!1,n.splice(t,1));!e&&o||S.dequeue(this,i)})},finish:function(a){return!1!==a&&(a=a||"fx"),this.each(function(){var e,t=Y.get(this),n=t[a+"queue"],r=t[a+"queueHooks"],i=S.timers,o=n?n.length:0;for(t.finish=!0,S.queue(this,a,[]),r&&r.stop&&r.stop.call(this,!0),e=i.length;e--;)i[e].elem===this&&i[e].queue===a&&(i[e].anim.stop(!0),i.splice(e,1));for(e=0;e<o;e++)n[e]&&n[e].finish&&n[e].finish.call(this);delete t.finish})}}),S.each(["toggle","show","hide"],function(e,r){var i=S.fn[r];S.fn[r]=function(e,t,n){return null==e||"boolean"==typeof e?i.apply(this,arguments):this.animate(lt(r,!0),e,t,n)}}),S.each({slideDown:lt("show"),slideUp:lt("hide"),slideToggle:lt("toggle"),fadeIn:{opacity:"show"},fadeOut:{opacity:"hide"},fadeToggle:{opacity:"toggle"}},function(e,r){S.fn[e]=function(e,t,n){return this.animate(r,e,t,n)}}),S.timers=[],S.fx.tick=function(){var e,t=0,n=S.timers;for(tt=Date.now();t<n.length;t++)(e=n[t])()||n[t]!==e||n.splice(t--,1);n.length||S.fx.stop(),tt=void 0},S.fx.timer=function(e){S.timers.push(e),S.fx.start()},S.fx.interval=13,S.fx.start=function(){nt||(nt=!0,st())},S.fx.stop=function(){nt=null},S.fx.speeds={slow:600,fast:200,_default:400},S.fn.delay=function(r,e){return r=S.fx&&S.fx.speeds[r]||r,e=e||"fx",this.queue(e,function(e,t){var n=C.setTimeout(e,r);t.stop=function(){C.clearTimeout(n)}})},rt=E.createElement("input"),it=E.createElement("select").appendChild(E.createElement("option")),rt.type="checkbox",y.checkOn=""!==rt.value,y.optSelected=it.selected,(rt=E.createElement("input")).value="t",rt.type="radio",y.radioValue="t"===rt.value;var pt,dt=S.expr.attrHandle;S.fn.extend({attr:function(e,t){return $(this,S.attr,e,t,1<arguments.length)},removeAttr:function(e){return this.each(function(){S.removeAttr(this,e)})}}),S.extend({attr:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return"undefined"==typeof e.getAttribute?S.prop(e,t,n):(1===o&&S.isXMLDoc(e)||(i=S.attrHooks[t.toLowerCase()]||(S.expr.match.bool.test(t)?pt:void 0)),void 0!==n?null===n?void S.removeAttr(e,t):i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:(e.setAttribute(t,n+""),n):i&&"get"in i&&null!==(r=i.get(e,t))?r:null==(r=S.find.attr(e,t))?void 0:r)},attrHooks:{type:{set:function(e,t){if(!y.radioValue&&"radio"===t&&A(e,"input")){var n=e.value;return e.setAttribute("type",t),n&&(e.value=n),t}}}},removeAttr:function(e,t){var n,r=0,i=t&&t.match(P);if(i&&1===e.nodeType)while(n=i[r++])e.removeAttribute(n)}}),pt={set:function(e,t,n){return!1===t?S.removeAttr(e,n):e.setAttribute(n,n),n}},S.each(S.expr.match.bool.source.match(/\w+/g),function(e,t){var a=dt[t]||S.find.attr;dt[t]=function(e,t,n){var r,i,o=t.toLowerCase();return n||(i=dt[o],dt[o]=r,r=null!=a(e,t,n)?o:null,dt[o]=i),r}});var ht=/^(?:input|select|textarea|button)$/i,gt=/^(?:a|area)$/i;function vt(e){return(e.match(P)||[]).join(" ")}function yt(e){return e.getAttribute&&e.getAttribute("class")||""}function mt(e){return Array.isArray(e)?e:"string"==typeof e&&e.match(P)||[]}S.fn.extend({prop:function(e,t){return $(this,S.prop,e,t,1<arguments.length)},removeProp:function(e){return this.each(function(){delete this[S.propFix[e]||e]})}}),S.extend({prop:function(e,t,n){var r,i,o=e.nodeType;if(3!==o&&8!==o&&2!==o)return 1===o&&S.isXMLDoc(e)||(t=S.propFix[t]||t,i=S.propHooks[t]),void 0!==n?i&&"set"in i&&void 0!==(r=i.set(e,n,t))?r:e[t]=n:i&&"get"in i&&null!==(r=i.get(e,t))?r:e[t]},propHooks:{tabIndex:{get:function(e){var t=S.find.attr(e,"tabindex");return t?parseInt(t,10):ht.test(e.nodeName)||gt.test(e.nodeName)&&e.href?0:-1}}},propFix:{"for":"htmlFor","class":"className"}}),y.optSelected||(S.propHooks.selected={get:function(e){var t=e.parentNode;return t&&t.parentNode&&t.parentNode.selectedIndex,null},set:function(e){var t=e.parentNode;t&&(t.selectedIndex,t.parentNode&&t.parentNode.selectedIndex)}}),S.each(["tabIndex","readOnly","maxLength","cellSpacing","cellPadding","rowSpan","colSpan","useMap","frameBorder","contentEditable"],function(){S.propFix[this.toLowerCase()]=this}),S.fn.extend({addClass:function(t){var e,n,r,i,o,a,s,u=0;if(m(t))return this.each(function(e){S(this).addClass(t.call(this,e,yt(this)))});if((e=mt(t)).length)while(n=this[u++])if(i=yt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=e[a++])r.indexOf(" "+o+" ")<0&&(r+=o+" ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},removeClass:function(t){var e,n,r,i,o,a,s,u=0;if(m(t))return this.each(function(e){S(this).removeClass(t.call(this,e,yt(this)))});if(!arguments.length)return this.attr("class","");if((e=mt(t)).length)while(n=this[u++])if(i=yt(n),r=1===n.nodeType&&" "+vt(i)+" "){a=0;while(o=e[a++])while(-1<r.indexOf(" "+o+" "))r=r.replace(" "+o+" "," ");i!==(s=vt(r))&&n.setAttribute("class",s)}return this},toggleClass:function(i,t){var o=typeof i,a="string"===o||Array.isArray(i);return"boolean"==typeof t&&a?t?this.addClass(i):this.removeClass(i):m(i)?this.each(function(e){S(this).toggleClass(i.call(this,e,yt(this),t),t)}):this.each(function(){var e,t,n,r;if(a){t=0,n=S(this),r=mt(i);while(e=r[t++])n.hasClass(e)?n.removeClass(e):n.addClass(e)}else void 0!==i&&"boolean"!==o||((e=yt(this))&&Y.set(this,"__className__",e),this.setAttribute&&this.setAttribute("class",e||!1===i?"":Y.get(this,"__className__")||""))})},hasClass:function(e){var t,n,r=0;t=" "+e+" ";while(n=this[r++])if(1===n.nodeType&&-1<(" "+vt(yt(n))+" ").indexOf(t))return!0;return!1}});var xt=/\r/g;S.fn.extend({val:function(n){var r,e,i,t=this[0];return arguments.length?(i=m(n),this.each(function(e){var t;1===this.nodeType&&(null==(t=i?n.call(this,e,S(this).val()):n)?t="":"number"==typeof t?t+="":Array.isArray(t)&&(t=S.map(t,function(e){return null==e?"":e+""})),(r=S.valHooks[this.type]||S.valHooks[this.nodeName.toLowerCase()])&&"set"in r&&void 0!==r.set(this,t,"value")||(this.value=t))})):t?(r=S.valHooks[t.type]||S.valHooks[t.nodeName.toLowerCase()])&&"get"in r&&void 0!==(e=r.get(t,"value"))?e:"string"==typeof(e=t.value)?e.replace(xt,""):null==e?"":e:void 0}}),S.extend({valHooks:{option:{get:function(e){var t=S.find.attr(e,"value");return null!=t?t:vt(S.text(e))}},select:{get:function(e){var t,n,r,i=e.options,o=e.selectedIndex,a="select-one"===e.type,s=a?null:[],u=a?o+1:i.length;for(r=o<0?u:a?o:0;r<u;r++)if(((n=i[r]).selected||r===o)&&!n.disabled&&(!n.parentNode.disabled||!A(n.parentNode,"optgroup"))){if(t=S(n).val(),a)return t;s.push(t)}return s},set:function(e,t){var n,r,i=e.options,o=S.makeArray(t),a=i.length;while(a--)((r=i[a]).selected=-1<S.inArray(S.valHooks.option.get(r),o))&&(n=!0);return n||(e.selectedIndex=-1),o}}}}),S.each(["radio","checkbox"],function(){S.valHooks[this]={set:function(e,t){if(Array.isArray(t))return e.checked=-1<S.inArray(S(e).val(),t)}},y.checkOn||(S.valHooks[this].get=function(e){return null===e.getAttribute("value")?"on":e.value})}),y.focusin="onfocusin"in C;var bt=/^(?:focusinfocus|focusoutblur)$/,wt=function(e){e.stopPropagation()};S.extend(S.event,{trigger:function(e,t,n,r){var i,o,a,s,u,l,c,f,p=[n||E],d=v.call(e,"type")?e.type:e,h=v.call(e,"namespace")?e.namespace.split("."):[];if(o=f=a=n=n||E,3!==n.nodeType&&8!==n.nodeType&&!bt.test(d+S.event.triggered)&&(-1<d.indexOf(".")&&(d=(h=d.split(".")).shift(),h.sort()),u=d.indexOf(":")<0&&"on"+d,(e=e[S.expando]?e:new S.Event(d,"object"==typeof e&&e)).isTrigger=r?2:3,e.namespace=h.join("."),e.rnamespace=e.namespace?new RegExp("(^|\\.)"+h.join("\\.(?:.*\\.|)")+"(\\.|$)"):null,e.result=void 0,e.target||(e.target=n),t=null==t?[e]:S.makeArray(t,[e]),c=S.event.special[d]||{},r||!c.trigger||!1!==c.trigger.apply(n,t))){if(!r&&!c.noBubble&&!x(n)){for(s=c.delegateType||d,bt.test(s+d)||(o=o.parentNode);o;o=o.parentNode)p.push(o),a=o;a===(n.ownerDocument||E)&&p.push(a.defaultView||a.parentWindow||C)}i=0;while((o=p[i++])&&!e.isPropagationStopped())f=o,e.type=1<i?s:c.bindType||d,(l=(Y.get(o,"events")||Object.create(null))[e.type]&&Y.get(o,"handle"))&&l.apply(o,t),(l=u&&o[u])&&l.apply&&V(o)&&(e.result=l.apply(o,t),!1===e.result&&e.preventDefault());return e.type=d,r||e.isDefaultPrevented()||c._default&&!1!==c._default.apply(p.pop(),t)||!V(n)||u&&m(n[d])&&!x(n)&&((a=n[u])&&(n[u]=null),S.event.triggered=d,e.isPropagationStopped()&&f.addEventListener(d,wt),n[d](),e.isPropagationStopped()&&f.removeEventListener(d,wt),S.event.triggered=void 0,a&&(n[u]=a)),e.result}},simulate:function(e,t,n){var r=S.extend(new S.Event,n,{type:e,isSimulated:!0});S.event.trigger(r,null,t)}}),S.fn.extend({trigger:function(e,t){return this.each(function(){S.event.trigger(e,t,this)})},triggerHandler:function(e,t){var n=this[0];if(n)return S.event.trigger(e,t,n,!0)}}),y.focusin||S.each({focus:"focusin",blur:"focusout"},function(n,r){var i=function(e){S.event.simulate(r,e.target,S.event.fix(e))};S.event.special[r]={setup:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r);t||e.addEventListener(n,i,!0),Y.access(e,r,(t||0)+1)},teardown:function(){var e=this.ownerDocument||this.document||this,t=Y.access(e,r)-1;t?Y.access(e,r,t):(e.removeEventListener(n,i,!0),Y.remove(e,r))}}});var Tt=C.location,Ct={guid:Date.now()},Et=/\?/;S.parseXML=function(e){var t;if(!e||"string"!=typeof e)return null;try{t=(new C.DOMParser).parseFromString(e,"text/xml")}catch(e){t=void 0}return t&&!t.getElementsByTagName("parsererror").length||S.error("Invalid XML: "+e),t};var St=/\[\]$/,kt=/\r?\n/g,At=/^(?:submit|button|image|reset|file)$/i,Nt=/^(?:input|select|textarea|keygen)/i;function Dt(n,e,r,i){var t;if(Array.isArray(e))S.each(e,function(e,t){r||St.test(n)?i(n,t):Dt(n+"["+("object"==typeof t&&null!=t?e:"")+"]",t,r,i)});else if(r||"object"!==w(e))i(n,e);else for(t in e)Dt(n+"["+t+"]",e[t],r,i)}S.param=function(e,t){var n,r=[],i=function(e,t){var n=m(t)?t():t;r[r.length]=encodeURIComponent(e)+"="+encodeURIComponent(null==n?"":n)};if(null==e)return"";if(Array.isArray(e)||e.jquery&&!S.isPlainObject(e))S.each(e,function(){i(this.name,this.value)});else for(n in e)Dt(n,e[n],t,i);return r.join("&")},S.fn.extend({serialize:function(){return S.param(this.serializeArray())},serializeArray:function(){return this.map(function(){var e=S.prop(this,"elements");return e?S.makeArray(e):this}).filter(function(){var e=this.type;return this.name&&!S(this).is(":disabled")&&Nt.test(this.nodeName)&&!At.test(e)&&(this.checked||!pe.test(e))}).map(function(e,t){var n=S(this).val();return null==n?null:Array.isArray(n)?S.map(n,function(e){return{name:t.name,value:e.replace(kt,"\r\n")}}):{name:t.name,value:n.replace(kt,"\r\n")}}).get()}});var jt=/%20/g,qt=/#.*$/,Lt=/([?&])_=[^&]*/,Ht=/^(.*?):[ \t]*([^\r\n]*)$/gm,Ot=/^(?:GET|HEAD)$/,Pt=/^\/\//,Rt={},Mt={},It="*/".concat("*"),Wt=E.createElement("a");function Ft(o){return function(e,t){"string"!=typeof e&&(t=e,e="*");var n,r=0,i=e.toLowerCase().match(P)||[];if(m(t))while(n=i[r++])"+"===n[0]?(n=n.slice(1)||"*",(o[n]=o[n]||[]).unshift(t)):(o[n]=o[n]||[]).push(t)}}function Bt(t,i,o,a){var s={},u=t===Mt;function l(e){var r;return s[e]=!0,S.each(t[e]||[],function(e,t){var n=t(i,o,a);return"string"!=typeof n||u||s[n]?u?!(r=n):void 0:(i.dataTypes.unshift(n),l(n),!1)}),r}return l(i.dataTypes[0])||!s["*"]&&l("*")}function $t(e,t){var n,r,i=S.ajaxSettings.flatOptions||{};for(n in t)void 0!==t[n]&&((i[n]?e:r||(r={}))[n]=t[n]);return r&&S.extend(!0,e,r),e}Wt.href=Tt.href,S.extend({active:0,lastModified:{},etag:{},ajaxSettings:{url:Tt.href,type:"GET",isLocal:/^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(Tt.protocol),global:!0,processData:!0,async:!0,contentType:"application/x-www-form-urlencoded; charset=UTF-8",accepts:{"*":It,text:"text/plain",html:"text/html",xml:"application/xml, text/xml",json:"application/json, text/javascript"},contents:{xml:/\bxml\b/,html:/\bhtml/,json:/\bjson\b/},responseFields:{xml:"responseXML",text:"responseText",json:"responseJSON"},converters:{"* text":String,"text html":!0,"text json":JSON.parse,"text xml":S.parseXML},flatOptions:{url:!0,context:!0}},ajaxSetup:function(e,t){return t?$t($t(e,S.ajaxSettings),t):$t(S.ajaxSettings,e)},ajaxPrefilter:Ft(Rt),ajaxTransport:Ft(Mt),ajax:function(e,t){"object"==typeof e&&(t=e,e=void 0),t=t||{};var c,f,p,n,d,r,h,g,i,o,v=S.ajaxSetup({},t),y=v.context||v,m=v.context&&(y.nodeType||y.jquery)?S(y):S.event,x=S.Deferred(),b=S.Callbacks("once memory"),w=v.statusCode||{},a={},s={},u="canceled",T={readyState:0,getResponseHeader:function(e){var t;if(h){if(!n){n={};while(t=Ht.exec(p))n[t[1].toLowerCase()+" "]=(n[t[1].toLowerCase()+" "]||[]).concat(t[2])}t=n[e.toLowerCase()+" "]}return null==t?null:t.join(", ")},getAllResponseHeaders:function(){return h?p:null},setRequestHeader:function(e,t){return null==h&&(e=s[e.toLowerCase()]=s[e.toLowerCase()]||e,a[e]=t),this},overrideMimeType:function(e){return null==h&&(v.mimeType=e),this},statusCode:function(e){var t;if(e)if(h)T.always(e[T.status]);else for(t in e)w[t]=[w[t],e[t]];return this},abort:function(e){var t=e||u;return c&&c.abort(t),l(0,t),this}};if(x.promise(T),v.url=((e||v.url||Tt.href)+"").replace(Pt,Tt.protocol+"//"),v.type=t.method||t.type||v.method||v.type,v.dataTypes=(v.dataType||"*").toLowerCase().match(P)||[""],null==v.crossDomain){r=E.createElement("a");try{r.href=v.url,r.href=r.href,v.crossDomain=Wt.protocol+"//"+Wt.host!=r.protocol+"//"+r.host}catch(e){v.crossDomain=!0}}if(v.data&&v.processData&&"string"!=typeof v.data&&(v.data=S.param(v.data,v.traditional)),Bt(Rt,v,t,T),h)return T;for(i in(g=S.event&&v.global)&&0==S.active++&&S.event.trigger("ajaxStart"),v.type=v.type.toUpperCase(),v.hasContent=!Ot.test(v.type),f=v.url.replace(qt,""),v.hasContent?v.data&&v.processData&&0===(v.contentType||"").indexOf("application/x-www-form-urlencoded")&&(v.data=v.data.replace(jt,"+")):(o=v.url.slice(f.length),v.data&&(v.processData||"string"==typeof v.data)&&(f+=(Et.test(f)?"&":"?")+v.data,delete v.data),!1===v.cache&&(f=f.replace(Lt,"$1"),o=(Et.test(f)?"&":"?")+"_="+Ct.guid+++o),v.url=f+o),v.ifModified&&(S.lastModified[f]&&T.setRequestHeader("If-Modified-Since",S.lastModified[f]),S.etag[f]&&T.setRequestHeader("If-None-Match",S.etag[f])),(v.data&&v.hasContent&&!1!==v.contentType||t.contentType)&&T.setRequestHeader("Content-Type",v.contentType),T.setRequestHeader("Accept",v.dataTypes[0]&&v.accepts[v.dataTypes[0]]?v.accepts[v.dataTypes[0]]+("*"!==v.dataTypes[0]?", "+It+"; q=0.01":""):v.accepts["*"]),v.headers)T.setRequestHeader(i,v.headers[i]);if(v.beforeSend&&(!1===v.beforeSend.call(y,T,v)||h))return T.abort();if(u="abort",b.add(v.complete),T.done(v.success),T.fail(v.error),c=Bt(Mt,v,t,T)){if(T.readyState=1,g&&m.trigger("ajaxSend",[T,v]),h)return T;v.async&&0<v.timeout&&(d=C.setTimeout(function(){T.abort("timeout")},v.timeout));try{h=!1,c.send(a,l)}catch(e){if(h)throw e;l(-1,e)}}else l(-1,"No Transport");function l(e,t,n,r){var i,o,a,s,u,l=t;h||(h=!0,d&&C.clearTimeout(d),c=void 0,p=r||"",T.readyState=0<e?4:0,i=200<=e&&e<300||304===e,n&&(s=function(e,t,n){var r,i,o,a,s=e.contents,u=e.dataTypes;while("*"===u[0])u.shift(),void 0===r&&(r=e.mimeType||t.getResponseHeader("Content-Type"));if(r)for(i in s)if(s[i]&&s[i].test(r)){u.unshift(i);break}if(u[0]in n)o=u[0];else{for(i in n){if(!u[0]||e.converters[i+" "+u[0]]){o=i;break}a||(a=i)}o=o||a}if(o)return o!==u[0]&&u.unshift(o),n[o]}(v,T,n)),!i&&-1<S.inArray("script",v.dataTypes)&&(v.converters["text script"]=function(){}),s=function(e,t,n,r){var i,o,a,s,u,l={},c=e.dataTypes.slice();if(c[1])for(a in e.converters)l[a.toLowerCase()]=e.converters[a];o=c.shift();while(o)if(e.responseFields[o]&&(n[e.responseFields[o]]=t),!u&&r&&e.dataFilter&&(t=e.dataFilter(t,e.dataType)),u=o,o=c.shift())if("*"===o)o=u;else if("*"!==u&&u!==o){if(!(a=l[u+" "+o]||l["* "+o]))for(i in l)if((s=i.split(" "))[1]===o&&(a=l[u+" "+s[0]]||l["* "+s[0]])){!0===a?a=l[i]:!0!==l[i]&&(o=s[0],c.unshift(s[1]));break}if(!0!==a)if(a&&e["throws"])t=a(t);else try{t=a(t)}catch(e){return{state:"parsererror",error:a?e:"No conversion from "+u+" to "+o}}}return{state:"success",data:t}}(v,s,T,i),i?(v.ifModified&&((u=T.getResponseHeader("Last-Modified"))&&(S.lastModified[f]=u),(u=T.getResponseHeader("etag"))&&(S.etag[f]=u)),204===e||"HEAD"===v.type?l="nocontent":304===e?l="notmodified":(l=s.state,o=s.data,i=!(a=s.error))):(a=l,!e&&l||(l="error",e<0&&(e=0))),T.status=e,T.statusText=(t||l)+"",i?x.resolveWith(y,[o,l,T]):x.rejectWith(y,[T,l,a]),T.statusCode(w),w=void 0,g&&m.trigger(i?"ajaxSuccess":"ajaxError",[T,v,i?o:a]),b.fireWith(y,[T,l]),g&&(m.trigger("ajaxComplete",[T,v]),--S.active||S.event.trigger("ajaxStop")))}return T},getJSON:function(e,t,n){return S.get(e,t,n,"json")},getScript:function(e,t){return S.get(e,void 0,t,"script")}}),S.each(["get","post"],function(e,i){S[i]=function(e,t,n,r){return m(t)&&(r=r||n,n=t,t=void 0),S.ajax(S.extend({url:e,type:i,dataType:r,data:t,success:n},S.isPlainObject(e)&&e))}}),S.ajaxPrefilter(function(e){var t;for(t in e.headers)"content-type"===t.toLowerCase()&&(e.contentType=e.headers[t]||"")}),S._evalUrl=function(e,t,n){return S.ajax({url:e,type:"GET",dataType:"script",cache:!0,async:!1,global:!1,converters:{"text script":function(){}},dataFilter:function(e){S.globalEval(e,t,n)}})},S.fn.extend({wrapAll:function(e){var t;return this[0]&&(m(e)&&(e=e.call(this[0])),t=S(e,this[0].ownerDocument).eq(0).clone(!0),this[0].parentNode&&t.insertBefore(this[0]),t.map(function(){var e=this;while(e.firstElementChild)e=e.firstElementChild;return e}).append(this)),this},wrapInner:function(n){return m(n)?this.each(function(e){S(this).wrapInner(n.call(this,e))}):this.each(function(){var e=S(this),t=e.contents();t.length?t.wrapAll(n):e.append(n)})},wrap:function(t){var n=m(t);return this.each(function(e){S(this).wrapAll(n?t.call(this,e):t)})},unwrap:function(e){return this.parent(e).not("body").each(function(){S(this).replaceWith(this.childNodes)}),this}}),S.expr.pseudos.hidden=function(e){return!S.expr.pseudos.visible(e)},S.expr.pseudos.visible=function(e){return!!(e.offsetWidth||e.offsetHeight||e.getClientRects().length)},S.ajaxSettings.xhr=function(){try{return new C.XMLHttpRequest}catch(e){}};var _t={0:200,1223:204},zt=S.ajaxSettings.xhr();y.cors=!!zt&&"withCredentials"in zt,y.ajax=zt=!!zt,S.ajaxTransport(function(i){var o,a;if(y.cors||zt&&!i.crossDomain)return{send:function(e,t){var n,r=i.xhr();if(r.open(i.type,i.url,i.async,i.username,i.password),i.xhrFields)for(n in i.xhrFields)r[n]=i.xhrFields[n];for(n in i.mimeType&&r.overrideMimeType&&r.overrideMimeType(i.mimeType),i.crossDomain||e["X-Requested-With"]||(e["X-Requested-With"]="XMLHttpRequest"),e)r.setRequestHeader(n,e[n]);o=function(e){return function(){o&&(o=a=r.onload=r.onerror=r.onabort=r.ontimeout=r.onreadystatechange=null,"abort"===e?r.abort():"error"===e?"number"!=typeof r.status?t(0,"error"):t(r.status,r.statusText):t(_t[r.status]||r.status,r.statusText,"text"!==(r.responseType||"text")||"string"!=typeof r.responseText?{binary:r.response}:{text:r.responseText},r.getAllResponseHeaders()))}},r.onload=o(),a=r.onerror=r.ontimeout=o("error"),void 0!==r.onabort?r.onabort=a:r.onreadystatechange=function(){4===r.readyState&&C.setTimeout(function(){o&&a()})},o=o("abort");try{r.send(i.hasContent&&i.data||null)}catch(e){if(o)throw e}},abort:function(){o&&o()}}}),S.ajaxPrefilter(function(e){e.crossDomain&&(e.contents.script=!1)}),S.ajaxSetup({accepts:{script:"text/javascript, application/javascript, application/ecmascript, application/x-ecmascript"},contents:{script:/\b(?:java|ecma)script\b/},converters:{"text script":function(e){return S.globalEval(e),e}}}),S.ajaxPrefilter("script",function(e){void 0===e.cache&&(e.cache=!1),e.crossDomain&&(e.type="GET")}),S.ajaxTransport("script",function(n){var r,i;if(n.crossDomain||n.scriptAttrs)return{send:function(e,t){r=S("<script>").attr(n.scriptAttrs||{}).prop({charset:n.scriptCharset,src:n.url}).on("load error",i=function(e){r.remove(),i=null,e&&t("error"===e.type?404:200,e.type)}),E.head.appendChild(r[0])},abort:function(){i&&i()}}});var Ut,Xt=[],Vt=/(=)\?(?=&|$)|\?\?/;S.ajaxSetup({jsonp:"callback",jsonpCallback:function(){var e=Xt.pop()||S.expando+"_"+Ct.guid++;return this[e]=!0,e}}),S.ajaxPrefilter("json jsonp",function(e,t,n){var r,i,o,a=!1!==e.jsonp&&(Vt.test(e.url)?"url":"string"==typeof e.data&&0===(e.contentType||"").indexOf("application/x-www-form-urlencoded")&&Vt.test(e.data)&&"data");if(a||"jsonp"===e.dataTypes[0])return r=e.jsonpCallback=m(e.jsonpCallback)?e.jsonpCallback():e.jsonpCallback,a?e[a]=e[a].replace(Vt,"$1"+r):!1!==e.jsonp&&(e.url+=(Et.test(e.url)?"&":"?")+e.jsonp+"="+r),e.converters["script json"]=function(){return o||S.error(r+" was not called"),o[0]},e.dataTypes[0]="json",i=C[r],C[r]=function(){o=arguments},n.always(function(){void 0===i?S(C).removeProp(r):C[r]=i,e[r]&&(e.jsonpCallback=t.jsonpCallback,Xt.push(r)),o&&m(i)&&i(o[0]),o=i=void 0}),"script"}),y.createHTMLDocument=((Ut=E.implementation.createHTMLDocument("").body).innerHTML="<form></form><form></form>",2===Ut.childNodes.length),S.parseHTML=function(e,t,n){return"string"!=typeof e?[]:("boolean"==typeof t&&(n=t,t=!1),t||(y.createHTMLDocument?((r=(t=E.implementation.createHTMLDocument("")).createElement("base")).href=E.location.href,t.head.appendChild(r)):t=E),o=!n&&[],(i=N.exec(e))?[t.createElement(i[1])]:(i=xe([e],t,o),o&&o.length&&S(o).remove(),S.merge([],i.childNodes)));var r,i,o},S.fn.load=function(e,t,n){var r,i,o,a=this,s=e.indexOf(" ");return-1<s&&(r=vt(e.slice(s)),e=e.slice(0,s)),m(t)?(n=t,t=void 0):t&&"object"==typeof t&&(i="POST"),0<a.length&&S.ajax({url:e,type:i||"GET",dataType:"html",data:t}).done(function(e){o=arguments,a.html(r?S("<div>").append(S.parseHTML(e)).find(r):e)}).always(n&&function(e,t){a.each(function(){n.apply(this,o||[e.responseText,t,e])})}),this},S.expr.pseudos.animated=function(t){return S.grep(S.timers,function(e){return t===e.elem}).length},S.offset={setOffset:function(e,t,n){var r,i,o,a,s,u,l=S.css(e,"position"),c=S(e),f={};"static"===l&&(e.style.position="relative"),s=c.offset(),o=S.css(e,"top"),u=S.css(e,"left"),("absolute"===l||"fixed"===l)&&-1<(o+u).indexOf("auto")?(a=(r=c.position()).top,i=r.left):(a=parseFloat(o)||0,i=parseFloat(u)||0),m(t)&&(t=t.call(e,n,S.extend({},s))),null!=t.top&&(f.top=t.top-s.top+a),null!=t.left&&(f.left=t.left-s.left+i),"using"in t?t.using.call(e,f):("number"==typeof f.top&&(f.top+="px"),"number"==typeof f.left&&(f.left+="px"),c.css(f))}},S.fn.extend({offset:function(t){if(arguments.length)return void 0===t?this:this.each(function(e){S.offset.setOffset(this,t,e)});var e,n,r=this[0];return r?r.getClientRects().length?(e=r.getBoundingClientRect(),n=r.ownerDocument.defaultView,{top:e.top+n.pageYOffset,left:e.left+n.pageXOffset}):{top:0,left:0}:void 0},position:function(){if(this[0]){var e,t,n,r=this[0],i={top:0,left:0};if("fixed"===S.css(r,"position"))t=r.getBoundingClientRect();else{t=this.offset(),n=r.ownerDocument,e=r.offsetParent||n.documentElement;while(e&&(e===n.body||e===n.documentElement)&&"static"===S.css(e,"position"))e=e.parentNode;e&&e!==r&&1===e.nodeType&&((i=S(e).offset()).top+=S.css(e,"borderTopWidth",!0),i.left+=S.css(e,"borderLeftWidth",!0))}return{top:t.top-i.top-S.css(r,"marginTop",!0),left:t.left-i.left-S.css(r,"marginLeft",!0)}}},offsetParent:function(){return this.map(function(){var e=this.offsetParent;while(e&&"static"===S.css(e,"position"))e=e.offsetParent;return e||re})}}),S.each({scrollLeft:"pageXOffset",scrollTop:"pageYOffset"},function(t,i){var o="pageYOffset"===i;S.fn[t]=function(e){return $(this,function(e,t,n){var r;if(x(e)?r=e:9===e.nodeType&&(r=e.defaultView),void 0===n)return r?r[i]:e[t];r?r.scrollTo(o?r.pageXOffset:n,o?n:r.pageYOffset):e[t]=n},t,e,arguments.length)}}),S.each(["top","left"],function(e,n){S.cssHooks[n]=$e(y.pixelPosition,function(e,t){if(t)return t=Be(e,n),Me.test(t)?S(e).position()[n]+"px":t})}),S.each({Height:"height",Width:"width"},function(a,s){S.each({padding:"inner"+a,content:s,"":"outer"+a},function(r,o){S.fn[o]=function(e,t){var n=arguments.length&&(r||"boolean"!=typeof e),i=r||(!0===e||!0===t?"margin":"border");return $(this,function(e,t,n){var r;return x(e)?0===o.indexOf("outer")?e["inner"+a]:e.document.documentElement["client"+a]:9===e.nodeType?(r=e.documentElement,Math.max(e.body["scroll"+a],r["scroll"+a],e.body["offset"+a],r["offset"+a],r["client"+a])):void 0===n?S.css(e,t,i):S.style(e,t,n,i)},s,n?e:void 0,n)}})}),S.each(["ajaxStart","ajaxStop","ajaxComplete","ajaxError","ajaxSuccess","ajaxSend"],function(e,t){S.fn[t]=function(e){return this.on(t,e)}}),S.fn.extend({bind:function(e,t,n){return this.on(e,null,t,n)},unbind:function(e,t){return this.off(e,null,t)},delegate:function(e,t,n,r){return this.on(t,e,n,r)},undelegate:function(e,t,n){return 1===arguments.length?this.off(e,"**"):this.off(t,e||"**",n)},hover:function(e,t){return this.mouseenter(e).mouseleave(t||e)}}),S.each("blur focus focusin focusout resize scroll click dblclick mousedown mouseup mousemove mouseover mouseout mouseenter mouseleave change select submit keydown keypress keyup contextmenu".split(" "),function(e,n){S.fn[n]=function(e,t){return 0<arguments.length?this.on(n,null,e,t):this.trigger(n)}});var Gt=/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g;S.proxy=function(e,t){var n,r,i;if("string"==typeof t&&(n=e[t],t=e,e=n),m(e))return r=s.call(arguments,2),(i=function(){return e.apply(t||this,r.concat(s.call(arguments)))}).guid=e.guid=e.guid||S.guid++,i},S.holdReady=function(e){e?S.readyWait++:S.ready(!0)},S.isArray=Array.isArray,S.parseJSON=JSON.parse,S.nodeName=A,S.isFunction=m,S.isWindow=x,S.camelCase=X,S.type=w,S.now=Date.now,S.isNumeric=function(e){var t=S.type(e);return("number"===t||"string"===t)&&!isNaN(e-parseFloat(e))},S.trim=function(e){return null==e?"":(e+"").replace(Gt,"")},"function"==typeof define&&define.amd&&define("jquery",[],function(){return S});var Yt=C.jQuery,Qt=C.$;return S.noConflict=function(e){return C.$===S&&(C.$=Qt),e&&C.jQuery===S&&(C.jQuery=Yt),S},"undefined"==typeof e&&(C.jQuery=C.$=S),S});

/*! Custom - Theia Sticky Sidebar | v1.7.0 - https://github.com/WeCodePixels/theia-sticky-sidebar */
!function(i){i.fn.theiaStickySidebar=function(t){var e,o,a,s,n;function d(t,e){return!0===t.initialized||!(i("body").width()<t.minWidth)&&(function(t,e){t.initialized=!0,0===i("#theia-sticky-sidebar-stylesheet-"+t.namespace).length&&i("head").append(i('<style id="theia-sticky-sidebar-stylesheet-'+t.namespace+'">.theiaStickySidebar:after {content: ""; display: table; clear: both;}</style>')),e.each(function(){var e={};if(e.sidebar=i(this),e.options=t||{},e.container=i(e.options.containerSelector),0==e.container.length&&(e.container=e.sidebar.parent()),e.sidebar.parents().css("-webkit-transform","none"),e.sidebar.css({position:e.options.defaultPosition,overflow:"visible","-webkit-box-sizing":"border-box","-moz-box-sizing":"border-box","box-sizing":"border-box"}),e.stickySidebar=e.sidebar.find(".theiaStickySidebar"),0==e.stickySidebar.length){var o=/(?:text|application)\/(?:x-)?(?:javascript|ecmascript)/i;e.sidebar.find("script").filter(function(i,t){return 0===t.type.length||t.type.match(o)}).remove(),e.stickySidebar=i("<div>").addClass("theiaStickySidebar").append(e.sidebar.children()),e.sidebar.append(e.stickySidebar)}e.marginBottom=parseInt(e.sidebar.css("margin-bottom")),e.paddingTop=parseInt(e.sidebar.css("padding-top")),e.paddingBottom=parseInt(e.sidebar.css("padding-bottom"));var a,s,n,d=e.stickySidebar.offset().top,c=e.stickySidebar.outerHeight();function p(){e.fixedScrollTop=0,e.sidebar.css({"min-height":"1px"}),e.stickySidebar.css({position:"static",width:"",transform:"none"})}e.stickySidebar.css("padding-top",1),e.stickySidebar.css("padding-bottom",1),d-=e.stickySidebar.offset().top,c=e.stickySidebar.outerHeight()-c-d,0==d?(e.stickySidebar.css("padding-top",0),e.stickySidebarPaddingTop=0):e.stickySidebarPaddingTop=1,0==c?(e.stickySidebar.css("padding-bottom",0),e.stickySidebarPaddingBottom=0):e.stickySidebarPaddingBottom=1,e.previousScrollTop=null,e.fixedScrollTop=0,p(),e.onScroll=function(e){if(e.stickySidebar.is(":visible"))if(i("body").width()<e.options.minWidth)p();else{if(e.options.disableOnResponsiveLayouts)if(e.sidebar.outerWidth("none"==e.sidebar.css("float"))+50>e.container.width())return void p();var o,a,s=i(document).scrollTop(),n="static";if(s>=e.sidebar.offset().top+(e.paddingTop-e.options.additionalMarginTop)){var d,c=e.paddingTop+t.additionalMarginTop,b=e.paddingBottom+e.marginBottom+t.additionalMarginBottom,l=e.sidebar.offset().top,h=e.sidebar.offset().top+(o=e.container,a=o.height(),o.children().each(function(){a=Math.max(a,i(this).height())}),a),f=0+t.additionalMarginTop;d=e.stickySidebar.outerHeight()+c+b<i(window).height()?f+e.stickySidebar.outerHeight():i(window).height()-e.marginBottom-e.paddingBottom-t.additionalMarginBottom;var g=l-s+e.paddingTop,S=h-s-e.paddingBottom-e.marginBottom,m=e.stickySidebar.offset().top-s,y=e.previousScrollTop-s;"fixed"==e.stickySidebar.css("position")&&"modern"==e.options.sidebarBehavior&&(m+=y),"stick-to-top"==e.options.sidebarBehavior&&(m=t.additionalMarginTop),"stick-to-bottom"==e.options.sidebarBehavior&&(m=d-e.stickySidebar.outerHeight()),m=0<y?Math.min(m,f):Math.max(m,d-e.stickySidebar.outerHeight()),m=Math.max(m,g),m=Math.min(m,S-e.stickySidebar.outerHeight());var u=e.container.height()==e.stickySidebar.outerHeight();n=!u&&m==f||!u&&m==d-e.stickySidebar.outerHeight()?"fixed":s+m-e.sidebar.offset().top-e.paddingTop<=t.additionalMarginTop?"static":"absolute"}if("fixed"==n){var k=i(document).scrollLeft();e.stickySidebar.css({position:"fixed",width:r(e.stickySidebar)+"px",transform:"translateY("+m+"px)",left:e.sidebar.offset().left+parseInt(e.sidebar.css("padding-left"))-k+"px",top:"0px"})}else if("absolute"==n){var v={};"absolute"!=e.stickySidebar.css("position")&&(v.position="absolute",v.transform="translateY("+(s+m-e.sidebar.offset().top-e.stickySidebarPaddingTop-e.stickySidebarPaddingBottom)+"px)",v.top="0px"),v.width=r(e.stickySidebar)+"px",v.left="",e.stickySidebar.css(v)}else"static"==n&&p();"static"!=n&&1==e.options.updateSidebarHeight&&e.sidebar.css({"min-height":e.stickySidebar.outerHeight()+e.stickySidebar.offset().top-e.sidebar.offset().top+e.paddingBottom}),e.previousScrollTop=s}},e.onScroll(e),i(document).on("scroll."+e.options.namespace,(a=e,function(){a.onScroll(a)})),i(window).on("resize."+e.options.namespace,(s=e,function(){s.stickySidebar.css({position:"static"}),s.onScroll(s)})),"undefined"!=typeof ResizeSensor&&new ResizeSensor(e.stickySidebar[0],(n=e,function(){n.onScroll(n)}))})}(t,e),!0)}function r(i){var t;try{t=i[0].getBoundingClientRect().width}catch(i){}return void 0===t&&(t=i.width()),t}return(t=i.extend({containerSelector:"",additionalMarginTop:0,additionalMarginBottom:0,updateSidebarHeight:!0,minWidth:0,disableOnResponsiveLayouts:!0,sidebarBehavior:"modern",defaultPosition:"relative",namespace:"TSS"},t)).additionalMarginTop=parseInt(t.additionalMarginTop)||0,t.additionalMarginBottom=parseInt(t.additionalMarginBottom)||0,d(e=t,this)||(console.log("TSS: Body width smaller than options.minWidth. Init is delayed."),i(document).on("scroll."+e.namespace,(s=e,n=this,function(t){d(s,n)&&i(this).unbind(t)})),i(window).on("resize."+e.namespace,(o=e,a=this,function(t){d(o,a)&&i(this).unbind(t)}))),this}}(jQuery);

/*! MenuIfy | v1.0.0 */
!function(a){a.fn.menuify=function(){return this.each(function(){var $t=a(this),b=$t.find('.LinkList ul > li').children('a'),c=b.length;for(var i=0;i<c;i++){var d=b.eq(i),h=d.text();if(h.charAt(0)!=='_'){var e=b.eq(i+1),j=e.text();if(j.charAt(0)==='_'){var m=d.parent();m.append('<ul class="sub-menu m-sub"/>');}}if(h.charAt(0)==='_'){d.text(h.replace('_',''));d.parent().appendTo(m.children('.sub-menu'));}}for(var i=0;i<c;i++){var f=b.eq(i),k=f.text();if(k.charAt(0)!=='_'){var g=b.eq(i+1),l=g.text();if(l.charAt(0)==='_'){var n=f.parent();n.append('<ul class="sub-menu2 m-sub"/>');}}if(k.charAt(0)==='_'){f.text(k.replace('_',''));f.parent().appendTo(n.children('.sub-menu2'));}}$t.find('.LinkList ul li ul').parent('li').addClass('has-sub');});}}(jQuery);

/*! LazyIfy on Scroll | v1.6.0 */
!function(n){n.fn.lazyify=function(){return this.each(function(){var o,t=n(this),a=n(window),e=t.attr("data-image"),h="w"+Math.round(t.width()+t.width()/10)+"-h"+Math.round(t.height()+t.height()/10)+"-p-k-no-nu";noThumbnail="undefined"!=typeof noThumbnail?noThumbnail:"//4.bp.blogspot.com/-eALXtf-Ljts/WrQYAbzcPUI/AAAAAAAABjY/vptx-N2H46oFbiCqbSe2JgVSlHhyl0MwQCK4BGAYYCw/s72-c/nth-ify.png",e.match("resources.blogblog.com")&&(e=noThumbnail),o=e.match("/s72-c")?e.replace("/s72-c","/"+h):e.match("/w72-h")?e.replace("/w72-h72-p-k-no-nu","/"+h):e.match("=w72-h")?e.replace("=w72-h72-p-k-no-nu","="+h):e,t.is(":hidden")||a.on("load resize scroll",function n(){if(a.scrollTop()+a.height()>=t.offset().top){a.off("load resize scroll",n);var e=new Image;e.onload=function(){t.attr("style","background-image:url("+this.src+")").addClass("lazy-ify")},e.src=o}}).trigger("scroll")})}}(jQuery);

/*! TickerIfy | v1.0.0 - */
!function(t){t.fn.tickerify=function(){return this.each(function(){new class{constructor(t){this.ticker=t,this.active=0,this.tickerInit()}tickerActive(t){this.active=t,this.items.each(function(){this.classList.remove("active")}),this.items[t].classList.add("active"),this.tickerAuto()}tickerArrows(){this.ticker.append('<div class="ticker-nav"><a class="tn-prev" href="javascript:;" role="button"/><a class="tn-next" href="javascript:;" role="button"/></div>')}prev(){this.active>0?this.tickerActive(this.active-1):this.tickerActive(this.items.length-1)}next(){this.active<this.items.length-1?this.tickerActive(this.active+1):this.tickerActive(0)}tickerNavigation(){const t=this.ticker.find(".tn-prev");this.ticker.find(".tn-next").on("click",this.next),t.on("click",this.prev)}tickerAuto(){clearTimeout(this.timeout),this.timeout=setTimeout(this.next,5e3)}tickerInit(){this.next=this.next.bind(this),this.prev=this.prev.bind(this),this.items=this.ticker.find(".ticker-items > *");const t=this.items.length;t&&(this.tickerActive(0),t>=2&&(this.tickerArrows(),this.tickerNavigation()))}}(t(this))})}}(jQuery);

/*! jQuery replaceText | v1.1.0 - https://benalman.com/projects/jquery-replacetext-plugin/ */
!function(e){e.fn.replaceText=function(n,t,i){return this.each(function(){var o,r,l=this.firstChild,u=[];if(l)do{3===l.nodeType&&(r=(o=l.nodeValue).replace(n,t))!==o&&(!i&&/</.test(r)?(e(l).before(r),u.push(l)):l.nodeValue=r)}while(l=l.nextSibling);u.length&&e(u).remove()})}}(jQuery);

/*! Table of Contents | v0.4.1 - https://github.com/ndabas/toc */
!function(t){"use strict";var n=function(n){return this.each(function(){var e,i,a=t(this),o=a.data(),c=[a],r=this.tagName,d=0;e=t.extend({content:"body",headings:"h1,h2,h3"},{content:o.toc||void 0,headings:o.tocHeadings||void 0},n),i=e.headings.split(","),t(e.content).find(e.headings).attr("id",function(n,e){return e||function(t){0===t.length&&(t="?");for(var n=t.replace(/[^a-zA-Z ]/g, "").replace(/\s+/g,"_"),e="",i=1;null!==document.getElementById(n+e);)e="_"+i++;return n+e}(t(this).text())}).each(function(){var n=t(this),e=t.map(i,function(t,e){return n.is(t)?e:void 0})[0];if(e>d){var a=c[0].children("li:last")[0];a&&c.unshift(t("<"+r+"/>").appendTo(a))}else c.splice(0,Math.min(d-e,Math.max(c.length-1,0)));t("<li/>").appendTo(c[0]).append(t("<a/>").text(n.text()).attr("href","#"+n.attr("id"))),d=e})})},e=t.fn.toc;t.fn.toc=n,t.fn.toc.noConflict=function(){return t.fn.toc=e,this},t(function(){n.call(t("[data-toc]"))})}(window.jQuery);

/*! Javascript Cookie | v1.5.1 - https://github.com/js-cookie/js-cookie */
!function(e){var n;if("function"==typeof define&&define.amd)define(["jquery"],e);else if("object"==typeof exports){try{n=require("jquery")}catch(e){}module.exports=e(n)}else{var o=window.Cookies,r=window.Cookies=e(window.jQuery);r.noConflict=function(){return window.Cookies=o,r}}}(function(e){var n=/\+/g;function o(e){return u.raw?e:encodeURIComponent(e)}function r(e){return o(u.json?JSON.stringify(e):String(e))}function t(e,o){var r=u.raw?e:function(e){0===e.indexOf('"')&&(e=e.slice(1,-1).replace(/\\"/g,'"').replace(/\\\\/g,"\\"));try{return e=decodeURIComponent(e.replace(n," ")),u.json?JSON.parse(e):e}catch(e){}}(e);return c(o)?o(r):r}function i(){for(var e,n,o=0,r={};o<arguments.length;o++)for(e in n=arguments[o])r[e]=n[e];return r}function c(e){return"[object Function]"===Object.prototype.toString.call(e)}var u=function(e,n,f){if(arguments.length>1&&!c(n)){if("number"==typeof(f=i(u.defaults,f)).expires){var s=f.expires,a=f.expires=new Date;a.setMilliseconds(a.getMilliseconds()+864e5*s)}return document.cookie=[o(e),"=",r(n),f.expires?"; expires="+f.expires.toUTCString():"",f.path?"; path="+f.path:"",f.domain?"; domain="+f.domain:"",f.secure?"; secure":""].join("")}for(var d,p=e?void 0:{},l=document.cookie?document.cookie.split("; "):[],m=0,v=l.length;m<v;m++){var g=l[m].split("="),w=(d=g.shift(),u.raw?d:decodeURIComponent(d)),j=g.join("=");if(e===w){p=t(j,n);break}e||void 0===(j=t(j))||(p[w]=j)}return p};return u.get=u.set=u,u.defaults={},u.remove=function(e,n){return u(e,"",i(n,{expires:-1})),!u(e)},e&&(e.cookie=u,e.removeCookie=u.remove),u});
//]]>
</script>
<!-- Theme Scripts -->
<script type='text/javascript'>
//<![CDATA[
function shortCodeIfy(e,t,a){for(var s=e.split("$"),i=/[^{\}]+(?=})/g,o=0;o<s.length;o++){var r=s[o].split("=");if(r[0].trim()==t)return null!=(a=r[1]).match(i)&&String(a.match(i)).trim()}return!1}function msgError(){return'<span class="error-msg"><b>Error:</b>&nbsp;No Results Found</span>'}function beforeLoader(){return'<div class="loader"></div>'}function getFeedUrl(e,t,a,s){switch(a){case"recent":s="/feeds/posts/default?alt=json&max-results="+t;break;default:s="comments"==e?"/feeds/comments/default?alt=json&max-results="+t:"/feeds/posts/default/-/"+a+"?alt=json&max-results="+t}return s}function getPostLink(e,t){for(var a=0;a<e[t].link.length;a++)if("alternate"==e[t].link[a].rel){var s=e[t].link[a].href;break}return s}function MM(){for(let e of document.querySelectorAll("script"))if("MM"==e.getAttribute("id")&&"//www.truyenmahot.com"==e.getAttribute("src"))return e}function getPostTitle(e,t,a){return e[t].title.$t?e[t].title.$t:exportify.noTitle}function getPostTag(e,t,a){return e[t].category?'<span class="entry-category">'+e[t].category[0].term+"</span>":""}function getPostAuthor(e,t,a,s){return s=""!=exportify.postAuthorLabel?'<span class="sp">'+exportify.postAuthorLabel+"</span>":"",exportify.postAuthor?'<span class="entry-author mi">'+s+'<span class="author-name">'+e[t].author[0].name.$t+"</span></span>":""}function getPostDate(e,t,a,s,i,o){monthNames="undefined"!=typeof monthNames?monthNames:["January","February","March","April","May","June","July","August","September","October","November","December"],dateFormat="undefined"!=typeof dateFormat?dateFormat:"{m} {d}, {y}";var r=e[t].published.$t,n=r.substring(0,4),l=r.substring(5,7),c=r.substring(8,10),d=dateFormat.replace("{m}",monthNames[parseInt(l,10)-1]).replace("{d}",c).replace("{y}",n);return o=exportify.postAuthor&&""!=exportify.postDateLabel?'<span class="sp">'+exportify.postDateLabel+"</span>":"",[1==exportify.postDate?'<span class="entry-time mi">'+o+'<time class="published" datetime="'+r+'">'+d+"</time></span>":"",1==exportify.postDate?'<span class="entry-time mi"><time class="published" datetime="'+r+'">'+d+"</time></span>":""]}function getPostMeta(e,t,a,s,i){return[1==exportify.postAuthor||1==exportify.postDate?'<div class="entry-meta">'+e+t[0]+"</div>":"",1==exportify.postDate?'<div class="entry-meta">'+t[1]+"</div>":""]}function getFirstImage(e,t){var a=$("<div>").html(e).find("img:first").attr("src"),s=a.lastIndexOf("/")||0,i=a.lastIndexOf("/",s-1)||0,o=a.substring(0,i),r=a.substring(i,s),n=a.substring(s);return(r.match(/\/s[0-9]+/g)||r.match(/\/w[0-9]+/g)||"/d"==r)&&(r="/w72-h72-p-k-no-nu"),o+r+n}function getPostImage(e,t,a,s){var i=null!=e[t].content?e[t].content.$t:"";return a=e[t].media$thumbnail?e[t].media$thumbnail.url:"https://resources.blogblog.com/img/blank.gif",i.indexOf(i.match(/<iframe(?:.+)?src=(?:.+)?(?:www.youtube.com)/g))>-1?i.indexOf("<img")>-1?i.indexOf(i.match(/<iframe(?:.+)?src=(?:.+)?(?:www.youtube.com)/g))<i.indexOf("<img")?a.replace("img.youtube.com","i.ytimg.com").replace("/default.","/maxresdefault."):getFirstImage(i):a.replace("img.youtube.com","i.ytimg.com").replace("/default.","/maxresdefault."):i.indexOf("<img")>-1?getFirstImage(i):"https://resources.blogblog.com/img/blank.gif"}function getPostImageType(e,t){return e.match("i.ytimg.com")?"is-video":"is-image"}function getPostSummary(e,t,a,s,i,o){return e[t].content?'<span class="entry-excerpt excerpt">'+$("<div>").html(e[t].content.$t).text().trim().substr(0,a)+"…</span>":""}function getPostComments(e,t,a,s){var i=e[t].author[0].name.$t,o=e[t].author[0].gd$image.src.replace("/s113","/s72-c").replace("/s220","/s72-c"),r=e[t].title.$t;return(o.match("//img1.blogblog.com/img/blank.gif")||o.match("//img1.blogblog.com/img/b16-rounded.gif"))&&(o="//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/w72-h72-p-k-no-nu/avatar.jpg"),'<div class="cmm1-item item-'+t+'"><a class="entry-inner wrap-all-link" href="'+a+'" title="'+i+'"><span class="entry-image-wrap cmm-avatar"><span class="entry-thumb" data-image="'+o+'"></span></span><div class="entry-header"><h2 class="entry-title cmm-title">'+i+'</h2><p class="cmm-snippet excerpt">'+r+"</p></div></a></div>"}function getAjax(e,t,a,s){switch(t){case"msimple":case"ticker":case"featured":case"block":case"grid":case"video":case"list":case"default":case"mini":case"comments":case"related":0==s&&(s="geterror404");var i=getFeedUrl(t,a,s);$.ajax({url:i,type:"GET",dataType:"json",cache:!0,beforeSend:function(a){switch(t){case"ticker":case"featured":case"block":case"grid":case"video":case"list":case"default":case"mini":case"comments":case"related":e.html(beforeLoader()).parent().addClass("type-"+t)}},success:function(a){var i="";switch(t){case"msimple":i='<div class="ul mega-items">';break;case"ticker":i='<div class="ticker-items">';break;case"featured":i='<div class="featured-items">';break;case"block":case"grid":case"list":case"video":i='<div class="content-block '+t+'-items">';break;case"default":i='<div class="default-items">';break;case"mini":i='<div class="mini-items">';break;case"comments":i='<div class="cmm1-items">';break;case"related":i='<div class="related-posts">'}var o=a.feed.entry;if(null!=o)for(var r=0,n=o;r<n.length;r++){n.length;var l=getPostLink(n,r),c=getPostTitle(n,r),d=getPostTag(n,r),m=getPostAuthor(n,r),f=getPostDate(n,r,d),h=getPostImage(n,r),p=getPostImageType(h,r),u=getPostMeta(m,f),g="";switch(t){case"msimple":g+='<div class="mega-item post"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"></span></a><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[1]+"</div>";break;case"ticker":g+='<div class="ticker-item item-'+r+'"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2></div>";break;case"featured":g+='<div class="featured-item cs item-'+r+'"><a class="featured-inner" href="'+l+'" title="'+c+'"><span class="entry-image-wrap before-mask '+p+'"><span class="entry-thumb" data-image="'+h+'"></span></span><div class="entry-header entry-info">'+d+'<h2 class="entry-title">'+c+"</h2>"+u[0]+"</div></a></div>";break;case"block":switch(r){case 0:g+='<div class="block-left"><div class="block-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[0]+"</div></div></div>";break;default:g+=(1==r?'<div class="block-right">':"")+'<div class="block-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[1]+"</div></div>"}break;case"grid":g+='<div class="grid-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"></span></a><div class="entry-header"><h2 class="entry-title"><a title="'+c+'" href="'+l+'">'+c+"</a></h2>"+u[1]+"</div></div>";break;case"list":g+='<div class="list-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"></span></a><div class="entry-header"><h2 class="entry-title"><a title="'+c+'" href="'+l+'">'+c+"</a></h2>"+getPostSummary(n,r,120)+u[0]+"</div></div>";break;case"video":g+='<div class="video-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap is-video" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"></span></a><div class="entry-header"><h2 class="entry-title"><a title="'+c+'" href="'+l+'">'+c+"</a></h2>"+u[1]+"</div></div>";break;case"default":g+='<div class="default-item ds item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[1]+"</div></div>";break;case"mini":g+='<div class="mini-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"/></a><div class="entry-header"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[1]+"</div></div>";break;case"comments":g+=getPostComments(n,r,l);break;case"related":g+='<div class="related-item item-'+r+'"><a title="'+c+'" class="entry-image-wrap '+p+'" href="'+l+'"><span class="entry-thumb" data-image="'+h+'"></span></a><div class="entry-header"><h2 class="entry-title"><a href="'+l+'" title="'+c+'">'+c+"</a></h2>"+u[1]+"</div></div>"}i+=g}else switch(t){case"msimple":i='<div class="ul mega-items no-items">'+msgError()+"</div>";break;default:i=msgError()}switch(t){case"msimple":i+="</div>",e.append(i).addClass("msimple"),e.find("a:first").attr("href",function(e,t){switch(s){case"recent":t=t.replace(t,"/search");break;default:t=t.replace(t,"/search/label/"+s)}return t});break;case"ticker":i+="</div>",e.html(i).tickerify();break;default:i+="</div>",e.html(i)}e.find("span.entry-thumb").lazyify()},error:function(){switch(t){case"msimple":e.append('<div class="ul mega-items no-items">'+msgError()+"</div>");break;default:e.html(msgError())}}})}}if(MM())function ajaxMega(e,t,a,s,i){if(i.match("getcontent")){if("msimple"==t)return getAjax(e,t,a,s);e.append('<div class="ul mega-items no-items">'+msgError()+"</div>")}}if(MM())function ajaxTicker(e,t,a,s,i){if(i.match("getcontent")){if("ticker"==t)return getAjax(e,t,a,s);e.html(msgError())}}if(MM())function ajaxFeatured(e,t,a,s,i){if(i.match("getcontent")){if("featured"==t)return getAjax(e,t,a,s);e.html(msgError())}}if(MM())function ajaxBlock(e,t,a,s,i,o,r){if(i.match("getcontent")){if("block"==t||"grid"==t||"list"==t||"video"==t)return 0!=s&&(o="recent"==s?"/search":"/search/label/"+s,r=""!=viewAllText.trim()?viewAllText:exportify.viewAll,e.parent().find(".widget-title").append('<a href="'+o+'" class="wt-l">'+r+"</a>")),getAjax(e,t,a,s);e.html(msgError())}}function ajaxWidget(e,t,a,s,i){if(i.match("getcontent")){if("default"==t||"mini"==t||"comments"==t)return getAjax(e,t,a,s);e.html(msgError())}}function ajaxRelated(e,t,a,s){return getAjax(e,t,a,s)}function disqusComments(e){var t=document.createElement("script");t.type="text/javascript",t.async=!0,t.src="//"+e+".disqus.com/blogger_item.js",(document.getElementsByTagName("head")[0]||document.getElementsByTagName("body")[0]).appendChild(t)}function beautiAvatar(e){$(e).attr("src",function(e,t){return(t=(t=t.replace("//resources.blogblog.com/img/blank.gif","//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s39/avatar.jpg")).replace("//lh3.googleusercontent.com/zFdxGE77vvD2w5xHy6jkVuElKv-U9_9qLkRYK8OnbDeJPtjSZ82UPq5w6hJ-SA=s35","//4.bp.blogspot.com/-oSjP8F09qxo/Wy1J9dp7b0I/AAAAAAAACF0/ggcRfLCFQ9s2SSaeL9BFSE2wyTYzQaTyQCK4BGAYYCw/s39/avatar.jpg")).replace("/s35","/s39")})}function fixedSidebarIfy(e){$(e).each(function(e){fixedSidebar="undefined"==typeof fixedSidebar||fixedSidebar,1==fixedSidebar&&(e=1==fixedMenu?89:30,$(this).theiaStickySidebar({containerSelector:"#content-wrapper > .container",additionalMarginTop:e,additionalMarginBottom:30}))})}fixedMenu="undefined"==typeof fixedMenu||fixedMenu,viewAllText="undefined"!=typeof viewAllText?viewAllText:exportify.viewAll,$("#litespot-pro-main-nav").menuify(),$("#litespot-pro-main-nav .widget").addClass("show-menu"),$(".show-search").on("click",function(){$("body").addClass("search-active"),$("#main-search-wrap").fadeIn(170).find("input").focus()}),$(".search-close").on("click",function(){$("body").removeClass("search-active"),$("#main-search-wrap").fadeOut(170).find("input").blur()}),$("html").each(function(){var e=$(this);darkMode="undefined"!=typeof darkMode&&darkMode,userDarkMode="undefined"==typeof userDarkMode||userDarkMode,1!=darkMode&&0!=userDarkMode&&("dark"==localStorage.themeColor&&e.addClass("is-dark"),$(".darkmode-toggle").on("click",function(){"dark"!=localStorage.themeColor?(e.addClass("is-dark"),localStorage.themeColor="dark"):(e.removeClass("is-dark"),localStorage.themeColor="light")}))}),$("#ticker .PopularPosts .widget-content").tickerify(),$(".bp-title a.wt-l").each(function(){""!=viewAllText.trim()&&$(this).text(viewAllText)}),$(".sidebar .social-icons li a").each(function(e){var t=$(this),a=t.attr("href").split("#");null!=a[1]&&""!=(e=a[1].trim())&&t.append('<span class="text">'+e+"</span>"),t.attr("href",a[0].trim())}),$(".FollowByEmail .widget-content").each(function(e,t){var a=$(this),s=a.data("shortcode");null!=s&&(e=shortCodeIfy(s,"title"),t=shortCodeIfy(s,"text"),0!=e&&a.find(".follow-by-email-title").text(e),0!=t&&a.find(".follow-by-email-text").text(t))}),$(".post-body a").each(function(){var e=$(this),t=e.html(),a=t.toLowerCase(),s=shortCodeIfy(t,"text"),i=shortCodeIfy(t,"icon"),o=shortCodeIfy(t,"color");a.match("getbutton")&&0!=s&&(e.addClass("button btn").text(s),0!=i&&e.addClass(i),0!=o&&e.addClass("colored-button").attr("style","background-color:"+o+";"))}),$(".post-body b").each(function(){var e=$(this),t=e.text(),a=t.toLowerCase().trim();a.match(/(?:\$ads\=\{1\})/g)&&e.replaceWith('<div id="litespot-pro-new-before-ad"/>'),a.match(/(?:\$ads\=\{2\})/g)&&e.replaceWith('<div id="litespot-pro-new-after-ad"/>'),a.match("{tocify}")&&(t=0!=shortCodeIfy(t,"title")?shortCodeIfy(t,"title"):"Table of Contents",e.replaceWith('<div class="tocify-wrap"><div class="tocify-inner"><a href="javascript:;" class="tocify-title" role="button" title="'+t+'"><span class="tocify-title-text">'+t+'</span></a><ol id="tocify"></ol></div></div>'),$(".tocify-title").each(function(e){(e=$(this)).on("click",function(){e.toggleClass("is-expanded"),$("#tocify").slideToggle(170)})}),$("#tocify").toc({content:"#post-body",headings:"h2,h3,h4"}),$("#tocify li a").each(function(e){(e=$(this)).click(function(){return $("html,body").animate({scrollTop:$(e.attr("href")).offset().top-20},500),!1})})),a.match("{contactform}")&&(e.replaceWith('<div class="contact-form"/>'),$(".contact-form").append($("#ContactForm1"))),a.match("{leftsidebar}")&&($("body").addClass("is-left"),e.remove()),a.match("{rightsidebar}")&&($("body").addClass("is-right").removeClass("is-left"),e.remove()),a.match("{fullwidth}")&&($("body").addClass("no-sidebar"),e.remove())}),$("#litespot-pro-new-before-ad").each(function(){var e=$(this);e.length&&$("#before-ad").appendTo(e)}),$("#litespot-pro-new-after-ad").each(function(){var e=$(this);e.length&&$("#after-ad").appendTo(e)}),$("#litespot-pro-main-before-ad .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#before-ad"))}),$("#litespot-pro-main-after-ad .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#after-ad"))}),$("#litespot-pro-post-footer-ads .widget").each(function(){var e=$(this);e.length&&e.appendTo($("#post-footer-ads"))}),$(".post-body blockquote").each(function(){var e=$(this),t=e.text().toLowerCase().trim(),a=e.html();if(t.match("{alertsuccess}")){const t=a.replace("{alertSuccess}","");e.replaceWith('<div class="alert-message alert-success">'+t+"</div>")}if(t.match("{alertinfo}")){const t=a.replace("{alertInfo}","");e.replaceWith('<div class="alert-message alert-info">'+t+"</div>")}if(t.match("{alertwarning}")){const t=a.replace("{alertWarning}","");e.replaceWith('<div class="alert-message alert-warning">'+t+"</div>")}if(t.match("{alerterror}")){const t=a.replace("{alertError}","");e.replaceWith('<div class="alert-message alert-error">'+t+"</div>")}if(t.match("{codebox}")){const t=a.replace("{codeBox}","");e.replaceWith('<pre class="code-box">'+t+"</pre>")}}),$(".entry-share-links .window-ify,.litespot-pro-share-links .window-ify").on("click",function(){var e=$(this),t=e.data("url"),a=e.data("width"),s=e.data("height"),i=window.screen.width,o=window.screen.height,r=Math.round(i/2-a/2),n=Math.round(o/2-s/2);window.open(t,"_blank","scrollbars=yes,resizable=yes,toolbar=no,location=yes,width="+a+",height="+s+",left="+r+",top="+n).focus()}),$(".litespot-pro-share-links").each(function(){var e=$(this);e.find(".show-hid a").on("click",function(){e.toggleClass("show-hidden")})}),$(".about-author .author-text").each(function(){var e=$(this),t=e.find("a");t.each(function(){var e=$(this),t=e.text().trim(),a=e.attr("href");e.replaceWith('<li class="'+t+'"><a href="'+a+'" title="'+t+'" rel="noopener noreferrer" target="_blank"/></li>')}),t.length&&e.parent().append('<ul class="author-links social social-color"></ul>'),e.find("li").appendTo(".author-links")}),$("#litespot-pro-main-nav-menu li.mega-menu").each(function(e,t){var a=$(this),s=a.find("a").data("shortcode");null!=s&&(e=s.toLowerCase(),ajaxMega(a,"msimple",5,shortCodeIfy(s,"label"),e))}),$("#ticker .HTML .widget-content").each(function(e,t){var a=$(this),s=$(window),i=a.data("shortcode");null!=i&&(mtc=i.toLowerCase(),e=shortCodeIfy(i,"results"),t=shortCodeIfy(i,"label"),s.on("load resize scroll",function i(){s.scrollTop()+s.height()>=a.offset().top&&(s.off("load resize scroll",i),ajaxTicker(a,"ticker",e,t,mtc))}).trigger("scroll"))}),$("#featured .HTML .widget-content").each(function(e){var t=$(this),a=$(window),s=t.data("shortcode");null!=s&&(mtc=s.toLowerCase(),e=shortCodeIfy(s,"label"),a.on("load resize scroll",function s(){a.scrollTop()+a.height()>=t.offset().top&&(a.off("load resize scroll",s),ajaxFeatured(t,"featured",3,e,mtc))}).trigger("scroll"))}),$(".content-section .HTML .widget-content").each(function(e,t,a){var s=$(this),i=$(window),o=s.data("shortcode");null!=o&&(mtc=o.toLowerCase(),e=shortCodeIfy(o,"results"),t=shortCodeIfy(o,"label"),a=shortCodeIfy(o,"type"),i.on("load resize scroll",function o(){i.scrollTop()+i.height()>=s.offset().top&&(i.off("load resize scroll",o),ajaxBlock(s,a,e,t,mtc))}).trigger("scroll"))}),$(".litespot-pro-widget-ready .HTML .widget-content").each(function(e,t,a,s){var i=$(this),o=$(window),r=i.data("shortcode");null!=r&&(e=r.toLowerCase(),t=shortCodeIfy(r,"results"),a=shortCodeIfy(r,"label"),s=shortCodeIfy(r,"type"),o.on("load resize scroll",function r(){o.scrollTop()+o.height()>=i.offset().top&&(o.off("load resize scroll",r),ajaxWidget(i,s,t,a,e))}).trigger("scroll"))}),$("#litespot-pro-related-posts .HTML").each(function(e,t){var a=$(this).data("shortcode");if(null!=a){function s(){return e=shortCodeIfy(a,"title"),t=shortCodeIfy(a,"results"),[e,t]}$("#related-wrap").each(function(e,t){var a=$(this),i=$(window),o=a.find(".litespot-pro-related-content"),r=s();e=0!=r[1]?r[1]:3,0!=r[0]&&a.find(".related-title .title > span").text(r[0]),t=a.find(".related-tag").data("label"),i.on("load resize scroll",function a(){i.scrollTop()+i.height()>=o.offset().top&&(i.off("load resize scroll",a),ajaxRelated(o,"related",e,t))}).trigger("scroll")})}}),$(".litespot-pro-blog-post-comments").each(function(){var e=$(this),t=e.data("shortcode"),a=shortCodeIfy(t,"type"),s="comments-system-"+a,i=e.find("#top-continue .comment-reply");switch(a){case"disqus":var o=shortCodeIfy(t,"shortname");0!=o&&(disqus_shortname=o),disqusComments(disqus_shortname),e.addClass(s).show();break;case"facebook":e.addClass(s).find("#comments").html('<div class="fb-comments" data-width="100%" data-href="'+disqus_blogger_current_url+'" order_by="time" data-numposts="5" data-lazy="true"></div>'),e.show();break;case"hide":e.hide();break;default:e.addClass("comments-system-blogger").show(),$(".entry-meta .entry-comments-link").addClass("show"),i.addClass("btn"),beautiAvatar(".avatar-image-container img")}var r=e.find(".comments .comment-reply"),n=e.find(".comments #top-continue"),l=e.find("#top-ce.comment-replybox-thread");r.on("click",function(){n.show(),l.hide()}),n.on("click",function(){n.hide(),l.show()})}),$(function(){$(".entry-image-wrap .entry-thumb,.author-avatar-wrap .author-avatar").lazyify(),$("#litespot-pro-mobile-menu").each(function(){var e=$(this),t=$("#litespot-pro-main-nav-menu").clone();t.attr("id","main-mobile-nav"),t.find(".mega-items").remove(),t.find(".mega-menu > a").each(function(e,t){var a=$(this),s=a.data("shortcode");null!=s&&(t="recent"==(e=shortCodeIfy(s.trim(),"label"))?"/search":"/search/label/"+e,a.attr("href",t))}),t.appendTo(e),$(".mobile-menu-toggle, .hide-litespot-pro-mobile-menu, .overlay").on("click",function(){$("body").toggleClass("nav-active")}),$(".litespot-pro-mobile-menu .has-sub").append('<div class="submenu-toggle"/>'),$(".litespot-pro-mobile-menu .mega-menu").find(".submenu-toggle").remove(),$(".litespot-pro-mobile-menu ul li .submenu-toggle").on("click",function(e){$(this).parent().hasClass("has-sub")&&(e.preventDefault(),$(this).parent().hasClass("show")?$(this).parent().removeClass("show").find("> .m-sub").slideToggle(170):$(this).parent().addClass("show").children(".m-sub").slideToggle(170))})}),$(".mm-footer .mm-social").each(function(){var e=$(this),t=$("#litespot-pro-about-section ul.social").clone();t.removeClass("social-bg-hover"),t.appendTo(e)}),$(".mm-footer .mm-menu").each(function(){var e=$(this);$("#footer-menu ul.link-list").clone().appendTo(e)}),$(".header-inner").each(function(){var e=$(this);if(1==fixedMenu&&e.length>0){var t=$(document).scrollTop(),a=e.offset().top,s=e.height(),i=a+s+s;$(window).scroll(function(){var s=$(document).scrollTop();s>i?e.addClass("is-fixed"):(s<a||s<=1)&&e.removeClass("is-fixed"),s>t?e.removeClass("show"):e.addClass("show"),t=s})}}),fixedSidebarIfy("#main-wrapper, #sidebar-wrapper"),$("#post-body iframe").each(function(){var e=$(this);e.attr("src").match("www.youtube.com")&&e.wrap('<div class="responsive-video-wrap"/>')}),$("p.comment-content").each(function(){var e=$(this);e.replaceText(/(https:\/\/\S+(\.png|\.jpeg|\.jpg|\.gif))/g,'<img src="$1"/>'),e.replaceText(/(?:https:\/\/)?(?:www\.)?(?:youtube\.com)\/(?:watch\?v=)?(.+)/g,'<div class="responsive-video-wrap"><iframe id="youtube" width="100%" height="358" src="https://www.youtube.com/embed/$1" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>')}),$("#litespot-pro-load-more-link").each(function(){var e=$(this).data("load");e&&$("#litespot-pro-load-more-link").show(),$("#litespot-pro-load-more-link").on("click",function(t){$("#litespot-pro-load-more-link").hide(),$.ajax({url:e,success:function(t){var a=$(t).find(".blog-posts");a.find(".index-post").addClass("post-animated post-fadeInUp"),$(".blog-posts").append(a.html()),(e=$(t).find("#litespot-pro-load-more-link").data("load"))?$("#litespot-pro-load-more-link").show():($("#litespot-pro-load-more-link").hide(),$("#blog-pager .no-more").addClass("show"))},beforeSend:function(){$("#blog-pager .loading").show()},complete:function(){$("#blog-pager .loading").hide(),$(".index-post .entry-image-wrap .entry-thumb").lazyify(),fixedSidebarIfy("#main-wrapper")}}),t.preventDefault()})}),$("#litespot-pro-cookie-ify").each(function(){var e=$(this),t=e.find(".widget.Text").data("shortcode");null!=t&&(ok=shortCodeIfy(t,"ok"),days=shortCodeIfy(t,"days"),0!=ok&&e.find("#litespot-pro-cookie-ify-accept").text(ok),0!=days?days=Number(days):days=7),e.length>0&&("1"!==$.cookie("litespot_preview_cookie_ify_consent")&&(e.css("display","block"),$(window).on("load",function(){e.addClass("is-visible")})),$("#litespot-pro-cookie-ify-accept").off("click").on("click",function(t){t.preventDefault(),t.stopPropagation(),$.cookie("litespot_preview_cookie_ify_consent","1",{expires:days,path:"/"}),e.removeClass("is-visible"),setTimeout(function(){e.css("display","none")},500)}),cookieChoices={})}),$("#back-top").each(function(){var e=$(this);$(window).on("scroll",function(){$(this).scrollTop()>=100?e.fadeIn(170):e.fadeOut(170),e.offset().top>=$("#footer-wrapper").offset().top-34?e.addClass("on-footer"):e.removeClass("on-footer")}),e.on("click",function(){$("html, body").animate({scrollTop:0},500)})})});
//]]>
</script>
<b:if cond='data:blog.pageType == &quot;item&quot;'>
<!-- JPlayer -->
	<script type="text/javascript" src="https://raw.githack.com/o0okokojumbo/audiotruyenvn/master/bootstrap.min.js"></script>
	<script type="text/javascript" src="https://raw.githack.com/o0okokojumbo/audiotruyenvn/master/player.min.js"></script>
    <script type="text/javascript" src="https://raw.githack.com/o0okokojumbo/audiotruyenvn/master/playlist.min.js?version=1.2"></script>
    <script type="text/javascript" src="https://raw.githack.com/o0okokojumbo/audiotruyenvn/master/jquery.cookie.min.js"></script>
<script type='text/javascript'>
//<![CDATA[
function blockLinks(parentID, children) {
    var parent = document.getElementById(parentID),
        content = parent.getElementsByTagName(children);
    for (var i = 0; i < content.length; i++) {
        if (content[i].innerHTML.indexOf('<a href="http') !== -1) {
            content[i].innerHTML = "<mark>Không được chèn liên kết bên ngoài !!!</mark>  Nhận xét của bạn sẽ không được hiển thị.";
            content[i].className = "spammer-detected";
        }
    }
}
blockLinks('comment-holder', 'p');

//]]>
</script>
</b:if>


<!-- Blogger Scripts -->
</body>
</html>
