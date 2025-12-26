Quantile [[clustering problem]] method ensures that each set will have an equal number of features in it where possible. If you have 1000 features, Quantile will stuff 250 into each of the four colors in your ramp. It’s the ice cube tray of thematic mapping, in that each cube (class) will be the same size no matter what is actually going on with the data. The advantage to this method is that it often excels at emphasizing the relative position of the data values (i.e., which counties contain the top 20 percent of the US population)

A quantile classification is well suited to linearly distributed data this because the resulting map can often be misleading. Similar features can be placed in adjacent classes, or features with widely different values can be put in the same class. You can minimize this distortion by increasing the number of classes.

# Bibliography

- ESRI https://pro.arcgis.com/en/pro-app/latest/help/mapping/layer-properties/data-classification-methods.htm
- some random book https://saylordotorg.github.io/text_essentials-of-geographic-information-systems/s10-03-data-classification.html
- ESRI Blog https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/better-breaks-define-your-thematic-maps-purpose/?rsource=https%3A%2F%2Flinks.esri.com%2Fbetter-breaks

