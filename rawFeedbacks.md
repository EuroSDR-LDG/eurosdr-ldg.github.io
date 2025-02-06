# Feedbacks 

### FB_BuildingChanges : Integrating topographic building data between two dates
contact/author : benedictebucher

This feedback is about the (#source data)  BDTopo data and (#source data)  ATKIS data on Strasbourg functional area, in 2011 and in 2021, only buildings. Users were a group of researchers in geomatics and our motivation was to map systematically the changes in buildings for densification studies

Feedback : we keep data in their source model, we applied a data-matching algorithm to match building features between 2011 and 2021. The tricky part is to identify mismatch that correspond to changes in the product (and not to changes in reality). The product detailed (#Source) documentation : https://geoservices.ign.fr/doc/DC_BDTOPO_3-0.pdf (in french) Quote of this document (p.24) : « Les bâtiments faisant entre 20 et 50 m² sont sélectionnés en fonction de leur environnement et de leur aspect. [..]Après unification de la BD TOPO® avec la BD PARCELLAIRE®, [..] il n’existe plus de seuil minimal pour la superficie des bâtiments. « 

### FB_MinetestTwin : Integrating data to generate a 3D interactive model
contact/author : indyteo

I used (#provider) IGN data to create a digital twin of the [#location: city of Loos-en-Gohelle (France)] as part of the (#funding program) CityFab project.

The goal was to [#usecase: create a 3D representation of the city in a simple environment, adapted for exploration, interaction and annotation from everyone], to meet the need of the municipality to organise a new modality of participatory democracy. The selected environment is the [#environment: game Minetest (Luanti)], which is supported by the digital working environment of every pupils (primary and secundary school) in France.

I integrated [#feature: DSM] from [#datasource: BD ALTI], [#feature: orthophoto] from [#datasource: BD ORTHO], [#feature: buildings footprints] and [#feature: roads] from [#datasource: BD TOPO], [#feature: buildings roofs] and [#feature: vegetation] from [#datasource: LIDAR HD] and [#feature: crops] from [#datasource: PRG].
One key challenge was to [#problem: match buildings footprints and buildings roofs], we faced alignment issues. We used the tool [#solution: Geoflow-Bundle to compute a single 3D model per building] by combining the two sources.

References:
- CityFab: https://www.univ-gustave-eiffel.fr/luniversite/nos-projets-transformants/city-fab (French)
- Minetest (Luanti): https://www.luanti.org/
- BD ALTI: https://geoservices.ign.fr/bdalti (French)
- BD ORTHO: https://geoservices.ign.fr/bdortho (French)
- BD TOPO: https://geoservices.ign.fr/bdtopo (French)
- LIDAR HD: https://geoservices.ign.fr/lidarhd (French)
- RPG: https://geoservices.ign.fr/rpg (French)
- Geoflow-Bundle: https://github.com/geoflow3d/geoflow-bundle

