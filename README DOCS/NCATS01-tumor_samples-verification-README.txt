NOTE: There are three files that hold sample data: NCATS01-tumor_samples.txt, NCATS01-normal_samples.txt, and NCATS01-blood_samples.txt.  But all three files contain the same columns, so only one file needed to be tested in order to test the Sample node in the database.  I chose to test NCATS01-tumor_samples.txt because it had the most data in the file.


analysis_area
- Type number
	- input string "notanumber" in row 6

analysis_area_percentage_glass
- Type number
	- input string "notanumber" in row 9

analysis_area_percentage_pigmented_tumor
- Type number
	- input string "notanumber" in row 10

analysis_area_percentage_stroma
- Type number
	- input string "notanumber" in row 8

analysis_area_percentage_tumor
- Type number
	- input string "notanumber" in row 7

comment
- Type string
	- no test possible

date-of_sample_collection
- Type datetime
	- no test possible

general_sample_pathology
- Type enum list (normal, tumor, (blood)): NOTE: blood was successfully input into database, but is not listed as a value in the enum list
	- input string "notinenumlist" in row 4
- Value required
	- left blank in row 5

length_of_tumor
- Type number
	- this field was not included in NCATS data - not tested

necropsy_sample
- Type boolean (loader accepted values Yes and No)
	- input string "notinenumlist" in row 16

non_tumor_tissue_area
- Type number
	- input string "notanumber" in row 13

percentage_stroma
- Type number
	- input string "notanumber" in row 15

percentage_tumor
- Type number
	- input string "notanumber" in row 14

sample_id
- Type string
	- not testable
- Value required
	- no value in row 1

sample_type
- Type enum list (tissue, blood)
	- input string "notinenumlist" in row 2
- Value required
	- no value in row 3

total_tissue_area
- Type number
	- input string "notanumber" in row 11

tumor_tissue_area
- Type number
	- input string "notanumber" in row 12

width_of_tumor
- Type number
	- this field was not included in NCATS data - not tested