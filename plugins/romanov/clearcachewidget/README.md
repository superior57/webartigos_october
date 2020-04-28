# Clear cache widget details
This report widget allows to clear OctoberCMS file cache with a single button click. 
> The widget works only if your system is configured to use the file cache driver, which stores the serialized, cached objects in the filesystem!

**[Clear cache widget](http://octobercms.com/plugin/romanov-clearcachewidget) on OctoberCMS marketplace.**

##### UI
You can display a widget with a chart or like a single button. Display options shown in the screenshots.

##### Features
- Clear cms cache
  + *cms/cache* 
  + *cms/combiner*
  + *cms/twig*
- Clear backend cache
  + *framework/cache*
- Clear thumbs cache of uploaded images

##### Available locales
- ru
- en
- pt-br (by [Leonardo Shinagawa](https://github.com/shina))
- cs (by [Vojta Svoboda](https://github.com/vojtasvoboda))
- fr (by [Jean Marc BRUNO](https://github.com/jimibi))
- it (by [Jean Marc BRUNO](https://github.com/jimibi))
- hu (by [Szabó Gergő](https://github.com/gergo85))
- tr (by [Sevdin Filiz](https://github.com/angelside))
- nl (by [Alwin Drenth](https://github.com/adrenth))
- sk (by [Marek Závacký](https://github.com/emzet))
- pl (by [Robert Pakszys](https://github.com/gorobert))

# Documentation

#### Installation
- The plugin can be installed from the Marketplace. Please see the details [here](http://octobercms.com/help/site/projects#introduction).  
- Install from backend:
  1. Go to "INSTALL PRODUCTS" page;
  2. Search plugin `Romanov.ClearCacheWidget` and install it.

  **After installation, you can add widget to dashboard.**

#### Widget configuration
- **Show without chart**  
Enable this option to display widget without chart.
- **Chart size**  
Radius value of chart. Optimal value is 200, but it's only my opinion :)
- **Delete thumbs images**  
If this option is enabled, thumbs of uploaded images also will be cleared.
- **Path to the folder with thumbs**  
Path to the folder in which stored thumbs cache. The path must be specified relative to the folder `storage`. Default value is `/app/uploads/public`.
- **Regex for thumb file names**  
Files with a name that matches the pattern will be deleted. For more details see [preg_match](http://php.net/manual/function.preg-match.php) function. Default value is `/^thumb_.*/`.
