# Web Service
   - Software component which can be accessed over network using a endpoint. 
   - ## Soap(Simple Object Access Protocol) based web service:
       - https://www.guru99.com/soap-simple-object-access-protocol.html. 
       - For portablity, uses a common format of message communication, xml.
       - WSDL(Web service definition language), consists of xml format of message, SOAP envelope.
       - Each soap envelope consists of
           - Header(authentication details)
           - Body(Name of the webservice, parameters required)
           - Fault element.
   - ## REST(Respresentational State Tranfer):
     - It is an architecture.
     - A RESTful web application exposes information about itself in the form of information about its resources. It also enables the client to take actions on those resources, such as create new resources (i.e. create a new user) or change existing resources.
      - When a RESTful API is called, the server will transfer to the client a representation of the state of the requested resource.
      - Representation- Format of data, State- Requested data.
      - Making a request:
        - Path to resource(HTTP URI)
          - Paths should contain the information necessary to locate a resource with the degree of specificity needed.
          - Use Nouns instead of Verbs.
          - Resource path examples:
             - /users <- user’s list
             - /users/123 <- specific user
             - /users/123/orders <- orders list that belongs to a specific user
             - /users/123/orders/0001 <- specific order of a specific user
          - Filtering, sorting, paging, and field selection:
             - GET /users?country=USA
             - GET /users?sort=birthdate_date:asc
             - GET /users?limit=100
        - Operation to perform on resource(CRUD ops specified using HTTP verb)
        - Optional Message body containing data
        - Optional Query param, Headers.
           
           
