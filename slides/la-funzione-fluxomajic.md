##  La funzione fluxomajic

```
http://localhost:8080/geoserver/wms?request=GetMap&service=WMS&version=1.1.1&layers=t4all%3Astrade&styles=traffico_fluxo
```

Stile del **visualizzatore smart**

```xml
<!-- Stile linea con algoritmo fluxomajic -->
<PolygonSymbolizer uom="http://www.opengeospatial.org/se/units/pixel">
    <Geometry>
        <ogc:Function name="fluxo">
            <ogc:PropertyName>shap</ogc:PropertyName>  <!-- Layer's attribute name -->
            <ogc:Literal>5</ogc:Literal>              <!-- Offset; expressed in pixel -->
            <ogc:Literal>5</ogc:Literal>              <!-- Width; expressed in pixel -->
            <ogc:Literal>0</ogc:Literal>              <!-- Drive side;   0 = RIGHT(default),
                                                                         1 = LEFT -->
            <ogc:Literal>4</ogc:Literal>              <!-- Number of quandrants (number of facets
                                                           into which to divide a fillet of
                                                           90 degrees);  16(default) -->
            <ogc:Literal>3</ogc:Literal>              <!-- ENDCAP style; 1 = ROUND(default),
                                                                         2 = FLAT,
                                                                         3 = SQUARE -->
            <ogc:Literal>1</ogc:Literal>              <!-- JOIN style;   1 = ROUND(default),
                                                                         2 = MITRE,
                                                                         3 = BEVEL -->
            <ogc:Literal>2</ogc:Literal>              <!-- Scaling Width (if the width has to scale
                                                           according to zoom level);
                                                                         1 = YES(default),
                                                                         2 = NO -->
            <ogc:Literal>3</ogc:Literal>            <!-- Minimum length (in pixel) of the diagonal
                                                      of the bounding box of the single geometry
                                                      to run the drawn process;  3(default) -->
            <ogc:Function name="env">                 <!-- envs (fixed and mandatory) -->
                <ogc:Literal>wms_crs</ogc:Literal>
            </ogc:Function>
            <ogc:Function name="env">
                <ogc:Literal>wms_width</ogc:Literal>
            </ogc:Function>
            <ogc:Function name="env">
                <ogc:Literal>wms_height</ogc:Literal>
            </ogc:Function>
            <ogc:Function name="env">
                <ogc:Literal>wms_bbox</ogc:Literal>
            </ogc:Function>
        </ogc:Function>
    </Geometry>
    <Fill>
        <CssParameter name="fill">
            <ogc:Literal>#33BA2E</ogc:Literal>
        </CssParameter>
    </Fill>
</PolygonSymbolizer>
```
