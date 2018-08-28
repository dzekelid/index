swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=BuildSuggesters:
    get:
      summary: Build Suggesters
      description: Indexes the search suggestions.
      operationId: BuildSuggesters
      x-api-path-slug: actionbuildsuggesters-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Suggesters
  /?Action=DefineIndexField:
    get:
      summary: Define Index Field
      description: Configures an ndexField  for the search domain.
      operationId: DefineIndexField
      x-api-path-slug: actiondefineindexfield-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: IndexField
        description: The index field and field options you want to configure
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=DeleteIndexField:
    get:
      summary: Delete Index Field
      description: "Removes an \n  IndexField\n  from the search domain."
      operationId: DeleteIndexField
      x-api-path-slug: actiondeleteindexfield-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      - in: query
        name: IndexFieldName
        description: The name of the index field your want to remove from the domains
          indexing options
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=DescribeIndexFields:
    get:
      summary: Describe Index Fields
      description: Gets information about the index fields configured for the search
        domain.
      operationId: DescribeIndexFields
      x-api-path-slug: actiondescribeindexfields-get
      parameters:
      - in: query
        name: Deployed
        description: Whether to display the deployed configuration (true) or include
          any pending changes (false)
        type: string
      - in: query
        name: DomainName
        description: The name of the domain you want to describe
        type: string
      - in: query
        name: FieldNames.member.N
        description: A list of the index fields you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Fields
  /?Action=IndexDocuments:
    get:
      summary: Index Documents
      description: Tells the search domain to start indexing its documents using the
        latest indexing options.
      operationId: IndexDocuments
      x-api-path-slug: actionindexdocuments-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Documents