1- patient_age_at_enrollment:
    Src: ENROLLMENT/ENROLL/1
    Type:
      units:
        - years
      value_type: number

		Test - Changed row 4 from a number to the word "Joker" (FAILED)

2- sex:
    Desc: gender, needs enum
    Src: ENROLLMENT/ENROLL/1
    Type:
    - M
    - F

		Test - Changed row 10 to "Hello." Going by the model, nothing should load from this file for sex. The model expects "M" or "F" and the values are coming in as "Male" and "Female" (FAILED)

3- neutered_indicator:
    Desc: Boolean indicator as to whther the patient has been either spayed (female patients)or neutered (male patients)
    Src: '?'
    Type: TBD

		Test - I don't think this is testable since the Type is TBD, but I changed row 2 from "Yes" to "Fred" in case it's expecting Yes or No. (PASSED)
			

4- weight:
    Desc: the subject's weight at the time the subject was enrolled and/or biospecimens were acquired, at least in the case of studies that are not longitudinal in nature
    Src: '?'
    Type: TBD

		Test - Not sure this is testable but I changed row 7 from a number to the word, "noneya"  (PASSED)
		

5-  breed:
    Src: ENROLLMENT/ENROLL/1
    Type:
    - http://localhost/terms/domain/breed

		Test - Changed row six from "Mixed Breed" to "6." (PASSED)
			

NOTE: None of the other properties in this node were being outputting in the transform, so no need to test. I also only tested the ones that had testable contraints (Type or Req)
