## EPCtagCoder


Java implementation of [EPC Tag Data Standard 1.9](http://www.gs1.org/epc/tag-data-standard)

An extremely intuitive, small and ultra fast EPC encoding and decoding library for java. 


### Example

```markdown


	ParseGDTI parseGDTI96 = ParseGDTI.Builder()
			   .withCompanyPrefix("0614141")
			   .withDocType("02346")
			   .withserial("274877906943") 
			   .withTagSize( GDTITagSize.BITS_96 )
			   .withFilterValue( GDTIFilterValue.ALL_OTHERS_0 )
			   .build();

	GDTI gdti96 = parseGDTI96.getGDTI();
	System.out.println("parseGDTI.getRfidTag()        "+ parseGDTI96.getRfidTag() );
	System.out.println("parseGDTI                     "+ gdti96.toString() );     
     

```

