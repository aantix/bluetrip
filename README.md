BlueTrip CSS Framework
=======================================

RAILS USAGE
-----------
Modified the image paths so that they match the default Rails 'images' directory.
Just copy the .css files to the public/stylesheets diretory and everything under
the img directory to the public/images directory.  Be sure to include the css files
in your application layout file.

github/bluetrip $ cp css/*.css ~/ProjectApp/public/stylesheets/
github/bluetrip $ cp -R img/* ~/ProjectApp/public/images/


app/views/layouts/application.html.erb

<head>
  <meta http-equiv="content-type" content="text/html;charset=UTF-8" />
  <title>Project Title</title>

  <%= stylesheet_link_tag 'screen', :media => 'screen, projection' %>
  <%= stylesheet_link_tag 'print', :media => 'print' %>
  <!--[if IE]>
      <link rel="stylesheet" href="/stylesheets/ie.css" type="text/css" media="screen, projection">
  <![endif]-->
  <%= stylesheet_link_tag 'style', :media => 'screen, projection' %>

</head>


A CSS Framework that fuses the best of Blueprint and Tripoli, among others.

USAGE
-----

Add the following four links to the <head> of your page::

    <link rel="stylesheet" href="../css/screen.css" type="text/css" media="screen, projection">
    <link rel="stylesheet" href="../css/print.css" type="text/css" media="print"> 
    <!--[if IE]>
        <link rel="stylesheet" href="../css/ie.css" type="text/css" media="screen, projection">
    <![endif]-->
    <link rel="stylesheet" href="../css/style.css" type="text/css" media="screen, projection">

Make sure you have the stylesheet links correct. 

Then edit "screen.css" to change `a[href^="http://yourwebsite.com"]` by putting your url in 
place of yourwebsite.com. This ensures that internal links will not show the external link icon.

Now get designing!

INFORMATION
-----------

Visit bluetrip.org for more detailed information, instructions, and support.

LICENSE
-------

See the LICENSE.txt file.

