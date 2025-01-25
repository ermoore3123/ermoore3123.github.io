# ermoore3123.github.io

Ethan R Moore, ermoore3@my.waketech.edu

this is my school github account

this repopsitory will hold my assighnments

# About Me

# My Interests
I'm a passionate student with a deep interest in computers and web development, especially front-end technologies like HTML, CSS, and JavaScript. Outside of coding, I love playing games, hiking, and exploring new languages and cultures. I’m always eager to learn new things and challenge myself with creative projects.

# Websites I Recommend

- [GitHub](https://www.github.com) - GitHub is a platform for version control in software development. I find it useful for hosting my projects, collaborating with other developers and contributing to open-source projects.
- [Stack Overflow](https://www.stackoverflow.com) - Stack Overflow is a great resource for getting help with coding problems and learning from other developers. 
- [MDN Web Docs](https://developer.mozilla.org) - MDN is my go-to resource for all things web development. Whether I’m learning a new thing or troubleshooting a bug, MDN has super accurate and well-documented information on HTML, CSS, JavaScript, and more.

# Additional Information
I'm currently working on improving my skills in machine learning and want to become good and all stuff computer. I also enjoy playing games and reading books.


erDiagram
    PRODUCT {
        string Productid PK
        string Name
        string Size
        string Color
        float Price
    }

    CUSTOMER {
        string Customerid PK
        string Name
        string Email
        string Phone
        string Address
    }

    SALE {
        string Saleid PK
        date Saledate
        float TotalAmount
        string PaymentMethod
        string CustomerID FK
        string ProductID FK
    }

    INVENTORY {
        string Inventoryid PK
        string Productid FK
        QuantityAvailable
    }

    CUSTOMMER ||--o| SALE: makes
    SALE ||--o| PRODUCT: contains
    PRODUCT ||--o| INVENTORY: StockedIn

Explanation of the ERD
Products to Sales: One product may appear in many sales, and one sale may include many products. This can be represented by the inclusion of a foreign key called ProductID in the SALE entity.

Customers to Sales: Each sale is related to one customer. Hence, one customer can have many sales. This is reflected in the inclusion of a foreign key called CustomerID in the SALE entity.

Product to Inventory: For each product, there will be a current stock level reflected in an inventory record. The ProductID foreign key will be included in the INVENTORY entity; therefore, one product can have only one inventory record for it-one-to-one relationship.