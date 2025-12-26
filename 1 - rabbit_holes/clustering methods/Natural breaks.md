The **Jenks optimization method**, also called the **Jenks natural breaks classification method**, is a [[clustering problem]] method designed to determine the best arrangement of values into different classes, the method seeks to reduce the variance within classes and maximize the variance between classes.

Because natural breaks classification places clustered values in the same class this method is best used with data that is unevenly distributed but not skewed toward either end of the distribution, One potential disadvantage is that this method can create classes that contain widely varying number ranges. Accordingly, class 1 is characterized by a range of just over 150,000, while class 5 is characterized by a range of over 6,000,000.
# How this method works

The method requires an iterative process. That is, calculations must be repeated using different breaks in the dataset to determine which set of breaks has the smallest in-class variance. The process is started by dividing the ordered data into classes in some way which may be arbitrary. There are two steps that must be repeated:

1. Calculate the sum of squared deviations from the class means (SDCM).
2. Choose a new way of dividing the data into classes, perhaps by moving one or more data points from one class to a different one.

New class deviations are then calculated, and the process is repeated until the sum of the within class deviations reaches a minimal value.

Alternatively, all break combinations may be examined, SDCM calculated for each combination, and the combination with the lowest SDCM selected. Since all break combinations are examined, this guarantees that the one with the lowest SDCM is found.

Reading this algorithm it's easy to detail that Natural breaks seems to be one dimensional [[k-means]]

# Bibliography

- Wikipedia https://en.wikipedia.org/wiki/Jenks_natural_breaks_optimization
- ESRI https://pro.arcgis.com/en/pro-app/latest/help/mapping/layer-properties/data-classification-methods.htm
- some random book https://saylordotorg.github.io/text_essentials-of-geographic-information-systems/s10-03-data-classification.html
- ESRI Blog https://www.esri.com/arcgis-blog/products/arcgis-online/mapping/better-breaks-define-your-thematic-maps-purpose/?rsource=https%3A%2F%2Flinks.esri.com%2Fbetter-breaks

