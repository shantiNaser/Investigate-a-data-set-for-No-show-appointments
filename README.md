# Introduction
Imagine that a person makes a doctor appointment, receives all the instructions, and then does not show up. Who is to blame? This is a significant issue, and we are here to analyze it and find solutions.

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
