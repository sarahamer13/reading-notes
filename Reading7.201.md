## In today's reading we learn how to use tables and the importance of using this and how it can allow us to pull specific data within an object ## 


### *Explain why we need domain modeling* ### 

- Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

### *Why should tables not be used for page layouts?* ###

- Layout tables reduce accessibility for visually impaired users: screen readers, used by blind people, interpret the tags that exist in an HTML page and read out the contents to the user. Because tables are not the right tool for layout, and the markup is more complex than with CSS layout techniques, the screen readers' output will be confusing to their users.

- Tables produce tag soup: As mentioned above, table layouts generally involve more complex markup structures than proper layout techniques. This can result in the code being harder to write, maintain, and debug.

- Tables are not automatically responsive: When you use proper layout containers (such as < header >, < section >, < article >, or < div >), their width defaults to 100% of their parent element. Tables on the other hand are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.


### *List and describe 3 different semantic HTML elements used in an HTML < table >* ###

- The smallest container inside a table is a table cell, which is created by a < td > element ('td' stands for 'table data')

- To stop this row from growing and start placing subsequent cells on a second row, we need to use the < tr > element ('tr' stands for 'table row')

- To recognize the table headers as headers, both visually and semantically, you can use the < th > element ('th' stands for 'table header'). This works in exactly the same way as a < td >, except that it denotes a header, not a normal cell. Go into your HTML, and change all the < td > elements surrounding the table headers into < th > elements.

### *What is a constructor and what are some advantages to using it?* ###

- A constructor is just a function 

- Using object literals is fine when you only need to create one object, but if you have to create more than one, as in the previous section, they're seriously inadequate. We have to write out the same code for every object we create, and if we want to change some properties of the object - like adding a height property - then we have to remember to update every object.

### *How does the term this differ when used in an object literal versus when used in a constructor?* ###

- AA constructor is just a function called using the new keyword. When you call a constructor, it will:

- create a new object
- bind this to the new object, so you can refer to this in your constructor code
- run the code in the constructor
- return the new object.

Constructors, by convention, start with a capital letter and are named for the type of object they create.


(Reference: Developer Mozilla)
(Github Codefellows)

## Things I want to know more about 

- how constructors work?
