## Servizi di Web Mapping e stili(2)

Funzioni e **trasformazioni geometriche** possono essere applicate alla componente geometrica del layer ed eseguite a runtime nello stile:

```xml
<!-- Estrazione vertici dal grafo stradale -->
<PointSymbolizer>
    <Geometry>
        <ogc:Function name="vertices">
            <ogc:PropertyName>the_geom</ogc:PropertyName>
        </ogc:Function>
    </Geometry>
    <Graphic>
        <Mark>
            <WellKnownName>square</WellKnownName>
                <Fill>
                    <CssParameter name="fill">#FF0000</CssParameter>
                </Fill>
        </Mark>
        <Size>6</Size>
    </Graphic>
</PointSymbolizer>
```
