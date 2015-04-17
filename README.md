# Map Lens

Map Lens is a sample JavaScript-based web application that demonstrates lensing or perhaps a better description is "draggable map insets".  Lensing offers many benefits over traditional swiping which is commonly used to horizontally transition between two web maps, for example, before and after a hurricane imagery.  In comparison, lensing offers the user an unlimited number of rectangular map overlays, for example, one lens per Esri basemap as shown above.

Click [here](http://richiecarmichael.github.io/lens/index.html) for the live application.

Lensing is achieved with the [ArcGIS API for JavaScript](https://developers.arcgis.com/javascript/) and leverages [jQuery](http://jquery.com/) and [jQueryUI](http://jqueryui.com/), specifically the [draggable](http://jqueryui.com/draggable/) and [resizeable](http://jqueryui.com/resizable/) methods.  The biggest challenge developing this sample was the handling (or suppressing) of the various mouse and navigation events.

Map lensing is not without its disadvantages.  Maps embedded in each lens cannot contain dynamic content, maps ideally should only contain tiled map or image service.  This is a performance consideration due to the number of navigation events invoked during lens interaction.

![](http://blogs.esri.com/esri/apl/files/2014/11/lens.gif =250x)
