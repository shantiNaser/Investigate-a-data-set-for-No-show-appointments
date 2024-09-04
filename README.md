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

  
# Visualization Area
   * The following visualizations have been generated from the analysis code to provide a clearer understanding of the key insights:
     <img width="913" alt="image" src="https://github.com/user-attachments/assets/238969df-c79f-4846-95b8-33f6f0302d2d">
     <img width="671" alt="image" src="https://github.com/user-attachments/assets/03e044f3-da5a-47c6-aaea-4c746e521357">


# Conclusions
After conducting a thorough analysis of the data, examining the variables, and identifying correlations, the following insights were obtained:
1. Key Factors for Predicting Patient Attendance:
    * Appointment Date: Appointments scheduled on Mondays or during holidays tend to have higher no-show rates. Therefore, the appointment date is a crucial factor.
    * Patient Age: Younger and older patients are more likely to miss their appointments, making age an important predictor.
    * No-Show History: Patients with a history of missed appointments are more likely to continue this behavior.
       * Recommendation: Implement a flagging system for patients with a history of no-shows to send reminders when they request future appointments.

2. Identifying Frequent No-Show Patients:
    * There are several patients who frequently schedule appointments but often fail to attend.
       * Recommendation: Identify and flag these patients to provide additional support or reminders for their appointments.

3. Average Age of No-Show Patients:
    * The analysis explored the average age of patients who do not attend their appointments to determine if younger patients are more likely to miss appointments.
       * Recommendation: Consider strategies that may be more effective in encouraging younger patients to attend, or adjust the scheduling criteria to prioritize older patients.

4. Impact of Neighborhood on No-Show Rates:
    * There are certain neighborhoods where no-show rates are significantly higher.
       * Recommendation: Investigate if specific neighborhoods, such as JARDIM CAMBURI during May, have underlying issues contributing to the higher no-show rates. Addressing these issues may help reduce missed appointments.

5. Importance of Appointment Reminders:
    * A significant number of patients (approximately 12,535) did not receive a reminder message before their appointment.
       * Recommendation: Ensure that reminder messages are sent to all patients before their appointments, as this could significantly reduce no-show rates.



# Reviwer Feedback
<img width="754" alt="image" src="https://github.com/user-attachments/assets/318193ae-930d-4657-9a80-ea51f0814a0a">

 


