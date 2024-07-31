# <p align="center">Flight Track<p>
   <p align="center">
   <p align="center"><strong>Home Page</strong></p>
   
## Project Summary

Description: Develop a system to provide real-time flight status updates and notifications to
passengers.
## Features

a. Real-time Updates: Display current flight status (delays, cancellations, gate
changes).
b. Push Notifications: Send notifications for flight status changes via SMS, email, or
app notifications you can use kafka, RabbitMQ , etc.
c. Integration with Airport Systems: Pull data from airport databases for accurate
information, we will give you mock data.

## Solution 

This project provides real-time flight status updates and notifications to users for tracking flights. Users can enter the date of the flight, flight number, airline, or simply the departure and arrival locations, with the only required field being the date of the flight. This flexibility allows users to search for flights easily.

Logged-in users can view the status of their booked flights without needing to search manually each time, enhancing convenience and efficiency.

The system provides real-time updates on current flight statuses, including delays, cancellations, and gate changes. Notifications about these status changes can be sent via SMS, email, and in-app messages. Kafka is used for in-app notifications to ensure reliable and efficient message delivery.

Integration with airport databases can be easily accomplished due to the use of SQL databases. The backend infrastructure is built using Python and PostgreSQL, with multiple databases managing user information, flight details, and bookings. Dynamic queries are used to handle multiple types of data, even if they are not included in the input.

Users are required to provide notification preferences during signup, which can be updated later by logging in. Users can select if they want to be notified about any changes in their flight plans. This feature ensures that users receive updates according to their preferences, making the system adaptable to individual needs.

 To keep track of status updates of a flight I had to make two different databases then compare them to check if the flight status is changed or not whenever its changed if the user has selected notification he will get notified ot the users who are not logged in can still check the status of particular flight by entering data,airline,departure airport,arrival airport etc

 user login and signup has password encryption with help of bycript and to handle messaging and email notification duties i had to use twilio and MIMEText to automate sending email to users. In frontend I had to build componet in react using MUI or Material-UI added multiple pages with link to redirected to homepage searching for flight out had a lot of options instead of being 

 dependent on a single flight number or date of flight user can choose a lot of things to search for his flight made seprate page for signup,login,inlogin(page you are redirected to after login )

## Screenshots

1. **Home Page**
  
   <p align="center">
      ![image](https://github.com/user-attachments/assets/5454b8cd-2796-4498-a75c-6edaace734e4)

   </p>
   <p align="center"><strong>Here user can enter Airline or Flight Number and Date to get status of their flight they get redirected to another page with all details of flight /strong></p>

3. **Flight Details**
   <p align="center">
      ![image](https://github.com/user-attachments/assets/a9ce435a-fc91-4c1a-8931-c366d09d367b)

   </p>
   <p align="center"><strong>Users can enter other details as well to search their flight with date being mandatory</strong></p>

4. **Login**
   <p align="center">
      ![image](https://github.com/user-attachments/assets/cc7bb8bb-7824-4620-a2e1-8562e0f2199a)

   </p>
   <p align="center"><strong>Users can login once they are signed up </strong></p>

5. **SignUp Page**
   <p align="center">
     ![image](https://github.com/user-attachments/assets/1922453f-abcb-4199-a34c-296a1ee65ac7)

   </p>
   <p align="center"><strong>SignUp Page</strong></p>



## How to Run the Project

1.  Clone the GitHub repository to your local machine.
2.  Configure environment variables for Twilio and email credentials.
3.  Install required packages using pip.
4.  Start the Flask server.
    ```
    python app.py
    ```
5. Install npm packages for React server.
    ```
    npm install -y
    ```
6. Start the React development server.
    ```
    npm run dev
    ```
