# Introduction
Imagine that a person makes a doctor's appointment, receives all the instructions, and then does not show up. Who is to blame? This is a significant issue, and we are here to analyze it and find solutions.

# Dataset Description
This dataset collects information from 110,527 medical appointments in Brazil and focuses on the question of whether or not patients show up for their appointments. Let's take a deep dive into each column and provide a detailed explanation of the data based on the descriptions given for each field:

* PatientId: Unique identifier assigned to each patient.
* AppointmentID: Unique identifier assigned for each appointment.
* Gender: Indicates the gender of the patient (Male or Female). The dataset notes a higher proportion of females, suggesting women tend to take better care of their health compared to men.
* DataMarcacaoConsulta: The actual date of the appointment, representing when the patient is scheduled to visit the doctor.
* DataAgendamento: The date on which the appointment was scheduled, always preceding or equal to the appointment date.
* Age: The age of the patient.
* Neighbourhood: The neighborhood where the appointment takes place.
* Scholarship: This is a binary field with values True or False, indicating whether the patient is enrolled in the Bolsa Família program, a Brazilian social welfare program. If you are interested, you can read more from this Link.
* Hipertension: This is a binary field with values True or False, indicating whether the patient has hypertension (high blood pressure).
* Diabetes: This is a binary field with values True or False, indicating whether the patient has diabetes.
* Alcoholism: This is a binary field with values True or False, indicating whether the patient has been diagnosed with alcoholism.
* Handcap: This is a binary field with values True or False, indicating if the patient has a disability.
* SMS_received: Indicates whether the patient received one or more SMS reminders about their appointment. Represented by a numeric value, typically 1 if one or more messages were sent, and 0 otherwise.
* No-show: This is a binary field with values True or False, indicating whether the patient attended the appointment, where True means the patient did not show up for the appointment, and False means they did.

# Conclusions
after a deep dive in the data, understanding variables, and finding the correlations I ended up with this result
1. What factors are important for us to know in order to predict if a patient will show up for their scheduled appointment?
    * appointments scheduled on Mondays or during holidays might have higher no-show rates. so Date is important
    * Younger or older patients might have higher no-show rates. age is also important
    * No-show History: Patients who have a history of missing appointments are likely to continue this behavior.
       * Note:- can we add a flag on this patient in order to notify him when he/she requests a new appointment later

2. Is there any patient who frequently schedules appointments but often does not show up?
    * yes there are many patients who have a Frequency of Appointments: as a solution Patients who schedule appointments frequently but often do not show up can be identified and flagged for additional appointments. 

3. What is the average old for the patients who schedule an appointments but does not show up?
    * I just asked this question in order to check if the Patient who registered is a Younger. So we can just accept the registration from older people

4. What is the Neighbourhood for the patient who scheduled an appointment but does not show up? Is there an issue with that Neighbourhood if it's frequently repeated for multiple patients for the same Neighbourhood
    * yes I have noticed that there are many Neighbourhood with no show-up patients reported
    * Example an idea:- we can check if there's an issue in JARDIM CAMBURI during May maybe inside this area or city since there's a lot of no show up appear in this month

5. does the Patient who does not show up to the appointment received a message before his appointment? if No what is the date on which the appointment was scheduled for him?
    * about 12535 users did not receive a message before their appointment -> so sending a message is very important
 


