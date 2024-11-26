# snackhub
- This a group project# bit2208-SE1-group-3

Members: 
Caroline Nduku Mbinda – BOBITNRB232523
Johnbosco Mueti – BOBITNRB318722
Faith Wanjiru Kiarii – BOBITNRB558122
Stephen Karanja Njoroge – BOBITNRB387822
Dan Mbuthia Waweru – BOBITLMR267120

Course Code  : BIT 2208
Unit Name    : Software Engineering I
Lecturer     : Cecilia Angela Nanfuka


Table of Content
    Description of the Mobile Application	       3
    Core Features	                               3
    Technical Implementation Plan	               4
    Software Requirements Specification (SRS)	   4
    Development Methodology	                     5
    Preferred Estimation Technique	             6
    Sequence Diagram for User Alerts	           6
    Sequence Diagram for Admin	                 7
   

Description of the Mobile Application
The Snacks Tuckshop mobile App is a user-friendly application designed to streamline the ordering process for its students and staff members. Its goal is to encourage students and staff members to explore, patronize, and order a variety of items beyond basic stationery, including snacks and treats during breaks between lectures. It aims to enhance the shopping experience by providing an engaging, user friendly interface and convenient features that align with the busy scheduled of all parties involved.
The app will  to serve as a digital platform for the Tuckshop to display its full range of products, allowing students to browse, place orders, and receive real-time updates on special offers and order status. The goal is to streamline the order process, increase sales, and improve user satisfaction through ease of use and accessibility.


Core Features
   •	Product Catalog: Displays a visually appealing catalog of all available Tuckshop items with detailed descriptions, images, and pricing.
   •	Real-time Inventory: Utilizing Firebase Realtime Database to maintain real-time inventory updates, ensuring accurate product availability. This will reduce the likelihood of users ordering unavailable products.
   •	Personalized Recommendations: Employing machine learning techniques (e.g., collaborative filtering) to analyze user preferences and suggest items based on past purchases and browsing history.
   •	Order Placement and Tracking: A seamless checkout process where users are allowed to  place orders directly through the app, track order status, and receive real-time notifications.
   •	Mobile Payments: Integrating with secure payment gateways to allow users to pay for their orders using various methods such as Mpesa or digital wallets, for seamless transactions.
   •	Loyalty Program: Implementing a reward system that incentivizes repeat purchases by offering points or discounts based on user activity within the app. This is to encourage repeat business.
   •	Push Notifications: Send targeted alerts / notifications for promotions, special offers, and order updates. (Alerts for limited-time offers and new arrivals)


Technical Implementation Plan
   •	Front-end Development: The user interface will be developed using Python frameworks such as Kivy or BeeWare that are suitable for mobile applications. These frameworks allow for cross-platform compatibility (iOS/Android).
   •	Back-end Development: Firebase will serve as the primary back-end service provider. It offers cloud storage solutions (Firestore), real-time database capabilities, authentication services (Firebase Auth), and hosting options. Tools to be used in conjunction with firebase include Flask or FastAPI for handling server-side logic while integrating with Firebase (i.e., to handle API requests, database interactions, and business logic.)
   •	Database Management: Firebase Firestore will be used to manage product listings, user profiles, order/transaction history, and inventory data in a structured manner.
   •	Authentication: Firebase Authentication will provide secure login options, thereby protecting user accounts. This will enable seamless sign-up and sign-in processes, and protect sensitive data.
   •	Application Programming Interface (API): Integration with payment processing APIs such as Mpesa for handling mobile payments securely.


Software Requirements Specification (SRS)
 The SRS outlines the functional and non-functional requirements essential for developing the mobile application:
   Functional Requirements:
      •	User account creation and authentication (Registration / Login);
      •	Display of product catalog with search and filter options (Product browsing);
      •	Real-time inventory updates
      •	Order placement
      •	Secure payment processing
      •	Order tracking
      •	Push notifications
      •	Loyalty Program Management
 
   Non-functional Requirements:
      •	Performance: fast load times and smooth navigation. The app should load within normal refresh rate,  under normal network conditions.
      •	Security: End-to-end encryption for data safety and secure payment processing.
      •	Reliability: high availability with minimal downtime. The system should have 99% uptime.
      •	Usability: the interface must be intuitive enough for first time users.
      •	Scalability: ability to handle increased user traffic during peak times


Development Methodology
Agile Methodology will be the guiding methodology due to its iterative approach allowing the development team to receive feedback, adjust features, and deliver parts of the product incrementally. This approach suits our proposed project as it will   require flexibility and user-centric development,  ensuring the final product meets the expectations and needs of our end-users.
Reasons for selecting Agile: 
   (.1.)	Flexibility and adaptability: University environments are dynamic, and requirements may change over time. Agile's iterative approach allows for flexibility to accommodate these changes without disrupting the project timeline. Additionally, agile emphasizes shorter development cycles, enabling quick feedback and adjustments to meet evolving user needs
   (.2.)	Prioritization and focus: Agile prioritizes the development of core features first, ensuring that the most valuable functionalities are delivered early. By delivering features in smaller increments, the team can focus on quality and user experience.
   (.3.)	Risk mitigation: frequent reviews and feedback sessions help identify and address potential risks early on. Agile's iterative nature allows for adjustments to the project plan as risks emerge (Adaptive Planning).
   (.4.)	Improve collaboration and communication: Agile promotes cross-functional partnership between developers, designers, and stakeholders, fostering a shared understanding of project goals. Additionally, frequent communication and feedback sessions ensure alignment and prevent misunderstandings.
   (.5.)	Enhanced User satisfaction: Agile encourages user involvement throughout the development process, leading to a product that better meets their needs. Iterative development allows for continuous improvement based on user feedback and testing.
Preferred Estimation Technique


Technique: User Story Pointing (USP) Method 
Reason: It is suitable for this project due to its flexibility in accommodating changes throughout the development cycle. It allows teams to estimate effort based on complexity rather than time; this is particularly beneficial where requirements may evolve based on user feedback or market trends. Additionally, it encourages collaborative discussions among team members about tasks’ complexities leading to more accurate estimations over time as teams become familiar with their velocity (the amount of work completed in a sprint). This method also allows prioritization of features based on business value rather than just technical difficulty


Sequence Diagram for User Alerts and Admin Duties
User: 
Below is a simple representation of how a user is alerted once their order is ready. It would include:
   (.1.)	User places an order through the mobile app;
   (.2.)	The app sends an order confirmation request to Firebase;
   (.3.)	Firebase processes the order request and updates inventory status;
   (.4.)	Once prepared, Firebase triggers a push notification alerting the user that their order is ready for pickup;
   (.5.)	The user’s device receives this notification via FCM (Firebase Cloud Messaging).
This flow ensures that users are kept informed throughout their purchasing journey while leveraging Firebase’s capabilities for real-time communication.

Admin
Below is a simple representation of correspondence on the admin side once an order is placed by the user. It would include:
   (.1.)	Admin views all placed orders;
   (.2.)	Admin updates the order status. 
This flow keeps the admin aware of what is taking place based on the number of user traffic to the site.
