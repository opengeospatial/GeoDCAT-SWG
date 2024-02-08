# Methodology Proposal for GeoDCAT

## Requirements identification

GeoDCAT can be incrementally developed from multiple existing applications in different forms to ensure adequate expressiveness to handle each case.

GeoDCAT-AP can be used for regression testing and to define a starting point, after refactoring to extract  requires after removal of all generic DCAT-AP artefacts and any EU-centric geographical elements

OGC-API-Records can be used as a baseline for OGC Catalog requirements, simply by mapping JSON schema elements to existing vocabularies such as DCAT, and examining if unmapped elements are appropriate for GeoDCAT scope.

STAC (and its various extensions) can be used the same way to determine other possible requirements - possibly mapped to extension profiles of GeoDCAT to manage scope.

Instances of ISO 19139 (or structured schemas using XML or other languages) can be translated using off-the-shelf tools to JSON then semantically mapped to DCAT, as per OGC API Records and STAC schema.

![](https://lucid.app/publicSegments/view/3f621317-a963-4159-bdec-af4602fa9751/image.png)

## Implementation Testing

Using the methodology above, concrete examples can be tested directly for transformability to GeoDCAT, and hence GeoDCAT capability to describe all elements deemed necessary to describe.
