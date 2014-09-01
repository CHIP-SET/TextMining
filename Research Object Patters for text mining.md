##Research Object pattern for Text mining###

###How to create an RO for your (source-code) software:
NB: there will be a number of RO design patterns e.g. executable or “non-executable” i.e. source code

Input: various things (code, papers, data, bla, bla)
Output: a (single) RO bundle  (potentially with external links)

1)	Write down your user stories
2)	Get a folder with your source code, papers, data, etc.
3)	Run something like ro-init/ro-add to create the initial manifest (with basic attributes plus aggregates)

```
"@context" : [ "https://w3id.org/bundle/context" ],
  "id" : "/",
  "manifest" : [ "/.ro/manifest.json" ],
  "createdOn" : "-",
  "createdBy" : [{"name":"Matthew Gamble",
    "orcidid": "http://orcid.org/0000-0003-4913-1485"}],
    "aggregates" : [
    {
      "file" : "/",
      "folder" : "/",
      "mediatype" : "application/vnd.robundle",
      "createdOn" : "2014-06-01T13:44:33.012Z",
      "proxy" : "urn:uuid:8a52f23b-24ff-41f9-a111-a138538c4567"
    },
```

4)	Add to the manifesto the attributes from the minimum check-list for that RO pattern
  a.	RO description (these would go in the ‘upper’ part of the manifesto)
    i.	RO ID (url, doi, purl, etc.) – Refer to SOME BEST PRACTICES HERE!
    ii.	Dublin CORE description for the source code 
      1.	Name of RO – DC:title
      2.	Author(s), date of creation, etc.
      3.	Description (textual) – this is DC:description so already included in DC
      4.	Keywords/tags (maybe tagged as whether it comes from a controlled vocabulary) - is this already in DC?
    iii.	Provenance (PAV)
    iv.	Versioning of the RO
    v.	Licensing for the RO
    vi.	Contact/maintainer
    vii.	Publication/documentation
  b.	Source-code-specific metadata (generally, these would go into the manifesto as annotations)
      i.	Software Ontology (but what is important from SO? E.g. versioning, license,  source, input, language, platform, dependencies, parameters, algorithm)
      ii.	Data (input/output) examples


 

### How to create an RO for your executable software:
NB: there will be a number of RO design patterns e.g. executable or “non-executable” i.e. source code

Input: various things (executable, papers, data, bla, bla)
Output: a (single) RO bundle (potentially with external links)

1)	Write down your user stories
2)	Get a folder with your executable image/file, papers, data, etc.
3)	Run something like ro-init/ro-add to create the initial manifest (with basic attributes plus aggregates)

4)	Add to the manifesto the attributes from the minimum check-list for that RO pattern
a.	RO description (these would go in the ‘upper’ part of the manifesto)
i.	RO ID (url, doi, purl, etc.) – Refer to SOME BEST PRACTICES HERE!
ii.	Dublin CORE description for the source code 
1.	Name of RO – DC:title
2.	Author(s), date of creation, etc.
3.	Description (textual) – this is DC:description so already included in DC
4.	Keywords/tags (maybe tagged as whether it comes from a controlled vocabulary) - is this already in DC?
iii.	Provenance (PROV)
iv.	Versioning of the RO
v.	Licensing for RO
vi.	Contact/maintainer
vii.	Publication 
b.	Software-executable-specific metadata (generally, these would go into the manifesto as annotations)
i.	Software Ontology (but what is important from SO? E.g. versioning, license,  source, input, language, platform, dependencies, parameters, algorithm)
ii.	Data (input/output) examples
iii.	Description of the executable platform (????)

 
The main to-dos

1)	Identify an initial CORE-RO minimal check-list, that is used across all RO types (software, datasets, workflows-methods)
2)	Prepare a CSV file with CORE-RO description for each of 3 use cases
3)	
