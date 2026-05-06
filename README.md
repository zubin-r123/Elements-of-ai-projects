# Elements of AI — Mini Projects

Projects completed as part of the 
[Elements of AI](https://www.elementsofai.com/) course by the 
University of Helsinki — one of the most widely recognised 
introductory AI programmes globally.

---

## About the Course

A free online course covering the fundamentals of AI — what it is,
what it can and can't do, and how it affects our lives. Completed
and certified in July 2023.

---

# Project Title

Disease prediction from selected set of symptoms

## Summary

Through this Project I want to propose a means by which a person is able to dignose themself in an emergency situation incase the is no healthcare professional available at the earliest. It gives people a rough idea of what they might be dealing with in terms of sickness through the AI predictor.It could save many lives and give many more people a sigh of relief.I hope this small idea can turn into something life changing and life saving in the near future!  


## Background

through this small algorithm of sorts, i want to be able to build a small ai model that can take symptoms as user inputs and be able to predict diseases and find appropriate medication prior to consulting a professional.I hope to build something that can be used at the household level and give people a second opinion as accurately as possible. 

what i want this model to solve is:
*giving people a better idea of what they might be dealing with medically
*give them a temporary solution they can refer to
*incase a doctor is not available at the earliest, this could be a trustworthy source for immediate consultation in the future
*it could also be helpful for doctors in the medical field as well


## How is it used?

The basic principle is that a user enters the symptoms they are going through and the AI model runs it through a sample set of symptoms that are connected to a set of possible diseases.The ai model then predicts the possible disease along with suggestions for medication

code example:
```
#this is a small sample code that i hope can be built into something bigger, more efficient and accurate
# Sample symptom and disease data
symptoms = [
    ["fever", "cough", "fatigue"],
    ["headache", "fever", "chills"],
    ["fatigue", "nausea", "vomiting"],
    # Add more symptom sets here
]

diseases = [
    "Common Cold",
    "Malaria",
    "Stomach Flu",
    # Add more diseases corresponding to symptom sets
]

# Create a dictionary to map symptoms to possible diseases
symptom_to_disease = {tuple(symptom_set): disease for symptom_set, disease in zip(symptoms, diseases)}

# Get input symptoms from the user
user_symptoms = input("Enter your symptoms separated by commas: ").split(',')

# Convert user symptoms to a tuple for dictionary lookup
user_symptoms_tuple = tuple(user_symptoms)

# Predict possible diseases
predicted_disease = symptom_to_disease.get(user_symptoms_tuple, "Unknown")

if predicted_disease != "Unknown":
    print(f"Based on your symptoms, you might have {predicted_disease}.")
else:
    print("Sorry, we couldn't determine a possible disease based on the provided symptoms.")

```


## Challenges

some ethical concerns would be that as humans we would not want to put our health in the hands of a machine, or whether this conultation technique is really worthwile.Both of these are valid arguements and fair reasons.Though  the impact a model like this could have would also be massively beneficial to a large amount of people.

## What next?

To make this project bigger and better i would like help with expanding the sample set as well as better integration between the sample set and the prediction system.



---

## Note

This repo represents early-stage AI learning. For my current 
AI engineering work, see the pinned repositories on my profile.
