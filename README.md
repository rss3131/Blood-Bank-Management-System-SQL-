# Blood-Bank-Management-System
My project focuses on the design of a database that stores the data for the Blood Bank Management System. This database includes all of the pertinent data required for each donation/transfusion, including the necessary pre-examination for the process.

SUMMARY!
This project focuses on the design of a database that stores the data for the Blood Bank Management System. The Blood Bank's primary focus is to facilitate the supply of blood to hospitals, health care clinics, medical and military facilities, educational centers, and research institutes, which save the patient's life. This database includes all of the pertinent data required for each donation/transfusion, including the necessary pre-examination for the process. A Blood bag entity shows the available stocks across all locations and can be narrowed down to a specific location. 

Blood Bank Management System keeps track of available blood when requested by an acceptor. Existing systems are manual, time-consuming, and are not so effective. Blood Bank Management System automates distribution capability. This database supports thousands of records for each blood bank. 

By using this system, searching the available blood becomes easy and saves a lot of time than the manual system. It will hoard, operate, recover, and analyze information concerned with the administrative and inventory management within a blood bank. I developed this system in a manageable manner to be time, cost, and resource-efficient, and that little human resource is needed.

MODEL WALKTHROUGH!

1.  Central Entity: In this model, the blood bag entity will be central to the database model. The relationships between the Donor and the Recipient and the requests are established through the blood bag entity. From the blood bag entity, any donation or transfusion takes place and is recorded. 

2.	The Three Specializations: 
The three different kinds of specializations are represented in my model.
1.	Separate subtype tables were utilized for the three main people in the Blood Bank Management System, i.e., Donor, Recipient, and the Nurse. This is favored for this scenario to distinguish the roles of each type of people. The Donor deals with donating the blood to the blood bank. The Recipient collects the blood from the blood bank for transfusion. The Nurse is the medical personnel assisting the complete process of blood bank management, so they have very specific and separate roles reflected in separate relationships. 
2.	The second specialization is the combination of the subtype tables and one supertype table. This was displayed in the relationships stemming from the blood bag entity, which serves as the supertype table. The subtypes are donation and transfusion records. The different types of services stored different data, but they also have common data and also a common set of relationships as blood bags. 
3.	The third specialization is the use of one table with the absence of subtype tables. The requests table characterizes this form of specialization. Keeping this as one table makes queries easy without leaving many unused columns. 
