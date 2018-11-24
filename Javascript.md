# Functions

## String with Underscores to CamelCase

​    const colName = "any_text_with_Underscores";

​    const colNameCamelCase = colName.replace(/_([a-z])/g, function (g) { return g[1].toUpperCase(); });

