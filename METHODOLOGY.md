# Methodology : scope and testing 

## Requirements identification

GeoDCAT can be incrementally developed from multiple existing applications in different forms to ensure adequate expressiveness to handle each case.

**The primary source of requirements for GeoDCAT will be existing standards for metadata for spatial data. Jurisdiction and domain-independent concepts will be identified or abstracted from such standards and included in GeoDCAT. Alignments to thes standards will be captured and published as part of the process to ensure transition and translation to/from GeoDCAT is fully supported by GeoDCAT design.**

[GeoDCAT-AP](https://semiceu.github.io/GeoDCAT-AP/drafts/latest/) can be used for regression testing and to define a starting point, after refactoring to extract requirements after removal of all generic [DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/) artefacts and any EU-centric geographical elements.

[OGC-API-Records](https://github.com/opengeospatial/ogcapi-records) can be used as a baseline for OGC Catalog requirements, simply by mapping JSON schema elements to existing vocabularies such as DCAT, and examining if unmapped elements are appropriate for GeoDCAT scope.  

[STAC](https://github.com/radiantearth/stac-spec) (and its various [extensions](https://github.com/stac-extensions)) can be used the same way to determine other possible requirements - possibly mapped to extension profiles of GeoDCAT to manage scope.

Instances of ISO 19139 (or structured schemas using XML or other languages) can be translated using off-the-shelf tools to JSON then semantically mapped to DCAT, as per OGC API Records and STAC schema.

![](https://lucid.app/publicSegments/view/0d5f7552-6631-4571-a631-4d085e088f1e/image.png)

## Implementation Testing

Using the methodology above, concrete examples can be tested directly for transformability to GeoDCAT, and hence GeoDCAT capability to define all elements deemed necessary to describe data sets.

The specification and testing of GeoDCAT profiles against OGC API and other standards occurs in a github repository [https://github.com/ogcincubator/geodcat-ogcapi-records](https://github.com/ogcincubator/geodcat-ogcapi-records) based on the OGC Building Blocks CI/CT (Continuous Integration/Continuous Testing) framework. 
