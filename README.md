# handlebars-asset-pipeline-example
Sample grails application with handlebars asset pipeline issue [#215](https://github.com/bertramdev/asset-pipeline/issues/215).

**Update 24/01/2015**
This issue is fixed in handlebars-asset-pipeline 2.0.0.1.

## Instructions

Using Grails 2.4.4, execute the following commands to reproduce the issue:

```
git clone https://github.com/tcrossland/handlebars-asset-pipeline-example.git
cd handlebars-asset-pipeline
grails war -verbose -stacktrace
```

## Result

```
...
.assetCompile:

|Precompiling Assets!
|Processing File 1 of 44 - apple-touch-icon-retina.png
|Processing File 2 of 44 - apple-touch-icon.png
|Processing File 3 of 44 - favicon.ico
|Compressing File 3 of 44 - favicon
|Processing File 4 of 44 - grails_logo.png
|Processing File 5 of 44 - skin/database_add.png
|Processing File 6 of 44 - skin/database_delete.png
|Processing File 7 of 44 - skin/database_edit.png
|Processing File 8 of 44 - skin/database_save.png
|Processing File 9 of 44 - skin/database_table.png
|Processing File 10 of 44 - skin/exclamation.png
|Processing File 11 of 44 - skin/house.png
|Processing File 12 of 44 - skin/information.png
|Processing File 13 of 44 - skin/shadow.jpg
|Processing File 14 of 44 - skin/sorted_asc.gif
|Processing File 15 of 44 - skin/sorted_desc.gif
|Processing File 16 of 44 - spinner.gif
|Processing File 17 of 44 - springsource.png
|Processing File 18 of 44 - application.js
   [delete] Deleting directory C:\Projects\handlebars-asset-pipeline-example\hbs\target\work\stage
.Error
|
WAR packaging error:
                        Handlebars Engine compilation of handlebars to javascript failed.
                        java.lang.NullPointerException: Cannot invoke method split() on null object
```
