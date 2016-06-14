CSV Spec:

Companies:

 

 

Customers:

Every customer has a maximum of 1 value for each of these fields: id,
first\_name, last\_name, title and company\_id  
Every customer can have multiple values for email, phone and address.  To
accommodate this, we have adopted the format as follows:

-   Emails - email\_home, email\_work, email\_mobile, email\_other

-   Phones - phone\_home, phone\_work, phone\_mobile, phone\_other

-   Addresses - address\_home, address\_work, address\_other

  
You can use as many of each as needed.  For example, if you have customers who
have 2 mobile phone numbers, its OK to have 2 columns named “phone\_mobile”.  


| **Column Name** | **Field Description** | **Desk Field** | **Data Type** | **Required** | **Unique** | **Validations**                                                            | **Example 1**                        | **Example 2**  |
|-----------------|-----------------------|----------------|---------------|--------------|------------|----------------------------------------------------------------------------|--------------------------------------|----------------|
| id              |                       | id             | String        | True         | True       |                                                                            | 8764387                              | Q3867          |
| first\_name     | Customer’s first      | first\_name    | String        | False        | False      |                                                                            | Jon                                  |                |
| last\_name      |                       | last\_name     | String        | False        | False      |                                                                            | Doe                                  |                |
| title           |                       | title          | String        | False        | False      |                                                                            | Mr.                                  |                |
| company\_id     |                       | company\_id    | String        | False        | False      | If value present, record with corresponding ID must exist in companies.csv | 655744                               |                |
| email\_home     |                       | email\_home    | String        | False        | True       |                                                                            | jon.doe\@gmail.com                   |                |
| email\_work     |                       | email\_work    | String        | False        | True       |                                                                            | jdoe\@work.com                       |                |
| email\_mobile   |                       | email\_mobile  | String        | False        | True       |                                                                            |                                      |                |
| email\_other    |                       | email\_other   | String        | False        | True       |                                                                            |                                      |                |
| phone\_home     |                       | phone\_home    | String        | False        | False      |                                                                            | 123-123-1234                         | (789) 234-5432 |
| phone\_work     |                       | phone\_work    | String        | False        | False      |                                                                            |                                      |                |
| phone\_mobile   |                       | phone\_mobile  | String        | False        | False      |                                                                            |                                      |                |
| phone\_other    |                       | phone\_other   | String        | False        | False      |                                                                            |                                      |                |
| address\_home   |                       | address\_home  | String        | False        | False      |                                                                            | 123 Main St, San Francisco, CA 94105 |                |
| address\_work   |                       | address\_work  | String        | False        | False      |                                                                            |                                      |                |
| address\_other  |                       | address\_other | String        | False        | False      |                                                                            |                                      |                |