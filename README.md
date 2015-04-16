SchemaOrg-Wikidata 
==================

*"[Schema.Org](http://www.Schema.Org) should have mappings to [Wikidata](https://www.wikidata.org) terms where possible"*: this is the recommendation expressed in [Git-SchemaOrg's issue #280](https://github.com/schemaorg/schemaorg/issues/280).

In order to comply with this recommendation, most of the mapping work must be performed "by humans", can't be automated. The "human interface" of this project is **[this GoogleDoc spreadsheet](https://docs.google.com/spreadsheets/d/1KeTSrVjSHRfVRwSgg6-LN0pu6nVre7cspUrkf_gfMm8/), any one can edit (!)**. Each month we check and transform the spreadsheet into a [simplifyed standard table, `data/humanInferences.csv`](https://github.com/ppKrauss/schemaOrg-wikidata/blob/master/data/humanInferences.csv).

The semantic of each SchemaOrg item is expressed by the item's descriptor (`rdfs:comment`) and tradition of use of the item in the SchemaOrg community. Each Wikidata-SchemaOrg map must be audited and confirmed by humans of the SchemaOrg community.

This project is a repo to the audited mappings (see `data/humanInferences.csv`) and a simple parser that enhance any version of the [schema_org_rdfa.html](http://schema.org/docs/schema_org_rdfa.html) definition with the mappings. 


## Formal mapping ##
*SchemaOrg* [is a RDF vocabulary](http://lov.okfn.org/dataset/lov/vocabs) and *Wikidata* is an ontology-database, a broader "formal representation of the knowledge by a set of concepts and the relationships between those concepts",[wikipedia](https://en.wikipedia.org/wiki/Ontology_(information_science)). The mappings can be expressed, in the *SchemaOrg* side, by [RDFa](https://en.wikipedia.org/wiki/RDFa#HTML.2BRDFa), **examples**:

* http://schema.org/Organization  is `owl:equivalentClass`  to *[Q43229](https://www.wikidata.org/wiki/Q43229)*.

* http://schema.org/City is `owl:equivalentClass`  to  *[Q515](https://www.wikidata.org/wiki/Q515)*.

* http://schema.org/Person is `owl:equivalentClass`  to *[Q215627](https://www.wikidata.org/wiki/Q215627)*.

* http://schema.org/PostalAddress is `owl:equivalentClass`  to  *[Q319608](https://www.wikidata.org/wiki/Q319608)*.

These equivalences was expressed in the table (spreadsheet) as:

...


------

... text and DEMO are under construction ...
