1- disease_term:
    Src: ENROLLMENT/ENROLL/1
    Type:
    - http://localhost/terms/domain/disease_term
    Req: true

		Test 1 - Removed the value in row 1 (FAILED)
		Test 2 - Put in ????? as the value in row 8  (PASSED)

2- pathology_report:
    Desc: Boolean indicator as to whether a detailed pathology report upon which the diagnosis was based exists
    Src: '?'
    Type: boolean

		Test 1 - removed "yes" in row 20 and added "Frank." Not sure this will break it (FAILED)

3- follow_up_data:
    Desc: Boolean indicator as to whether follow up data for the patient exists
    Src: '?'
    Type: boolean

		Test 1- removed "yes" in row 21 and added "Hello." Not sure this will break it (FAILED)

4-  treatment_data:
    Desc: Boolean indicator as to whether treatment data for the patient exists
    Src: '?'
    Type: boolean

		Test 1- removed "yes" in row 22 and added "awesome." Not sure this will break it (FAILED)

5-  concurrent_disease:
    Desc: Boolean indicator as to whether the patient is has any significant secondary disease condition(s)
    Src: '?'
    Type: boolean

		Test 1- removed "no" in row 23 and added "Claire." Not sure this will break it (FAILED)

6- histological_grade:
    Src: ENROLLMENT/ENROLL/1
    Type:
    - http://localhost/terms/domain/histological_grade

		Test 1- removed "III" in row 18 and put in "Kevin" as the value. I don't think this will break it. (PASSED)

7- primary_disease_site:
    Src: ENROLLMENT/ENROLL/1
    Type:
    - http://localhost/terms/domain/primary_disease_site

		Test 1- removed "Tibia" in row 15 and replaced it with the value "7." Not sure this will break it. (PASSED)


NOTE: All other props weren't testable because we either didn't output them or they have no requirments or other constraints like type or a list of values accepted