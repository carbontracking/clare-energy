# clare-energy
The Clare Community Energy Agency website

1. A navigation bar across the top that gives access to different pages
2. The possibility that one or more of those pages will display content like news/blog. This page will be created dynamically for content created elsewhere of type news/blog etc.
3. The ability for create users (by the admin) and/or that users can connect and create an account.
4. The ability to handle forms. 
    * This may be either generic forms that can be opened to the public (during a zoom for example) or forms that can be made available in user profiles.
    * The main data tables are
        * Users : who will have a number of fields (Name  /Email /Eircode /BER rating) and then specific fields depending on the project(s) they are involved in.
        * Projects : A project is like the Solar Meitheal for example. A project will have multiple users and some own data like DateStart , DateEnd, Name, Type
            * Users are connected to projects by the admin
        * Suppliers : Each supplier can be linked to one or more projects. Suppliers will have fields like name, address, eircode, Type (this will be things like BER / PV /Insulation etc.)
        * For each project there will also be separate UserData and SupplierData tables. e.g. Project1UserData  /Project1SupplierData. 
            * These will be created on a per project basis and the fields wil depend on the type of the project. 
            * When a User connects they will see the data fields for each project to which they are connected, likewise for the Suppliers
5. Forums : Each user will have default access to forums. If they have not been connected to a project then they only have read access, otherwise they will have read/write access.
