## Servizi di Web Mapping e stili

Pubblicazione di un layer con n differenti stili richiamabili a runtime

```
http://localhost:8080/geoserver/wms?request=GetMap&service=WMS&version=1.1.1&layers=t4all%3Astrade&styles=traffico_base
```

Stili **SLD** e **CSS**

```xml
<!-- Stile linea con classificazione stradale -->
<FeatureTypeStyle>
 <Rule>
   <Name>strada-locale</Name>
   <ogc:Filter>
     <ogc:PropertyIsEqualTo>
       <ogc:PropertyName>tipo</ogc:PropertyName>
       <ogc:Literal>strada-locale</ogc:Literal>
     </ogc:PropertyIsEqualTo>
   </ogc:Filter>
   <LineSymbolizer>
     <Stroke>
       <CssParameter name="stroke">#009933</CssParameter>
       <CssParameter name="stroke-width">2</CssParameter>
     </Stroke>
   </LineSymbolizer>
 </Rule>
</FeatureTypeStyle>
```

