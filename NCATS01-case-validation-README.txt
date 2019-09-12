1- patient_id:
    Desc: ID by which data owner can uniquely identify a specific patient, at least within a single study/trial, maintained exactly in the submitter's format. This may or may not be globally unique. 
    Src: ENROLLMENT/ENROLL/1
    Type: string
    Req: true
		Test - Row 1 was left blank for patient_id

2- case_id:
    Desc: globally unique ID by which the system can unambiguously identify and display a specific patient even across studies/trials. Likely to be a concatenation of a study identifier and patient_id below.
    Src: to be provided by the data submitter, generated during data transformation as necessary
    Type: string
    Req: true
	
		Test - Row 6 was left blank for case_id


NOTE: All other properties listed on this node were not testable because they were either strings or not required (no constraints).