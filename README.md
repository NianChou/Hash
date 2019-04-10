# Hash
## Hashing and Recovery of Original String API Services
THe API services for central are listed below:

1.  Convert Reference ID (RefID) to Record (Rec)
  1.	Parameters passed from client:

a.	NRIC Hashed value (RefID): alphanumeric 100

2.	Return value :

a.	NRIC (Rec): alphanumeric 100

II.	Function call to do batch conversion from Reference ID (RefID) to Record (Rec)

1.	Parameters passed from client:

a.	Application Record ID: alphanumeric 100

b.	NRIC hashed value (RefID): alphanumeric 100

2.	Return value :

a.	NRIC hashed value (RefID): alphanumeric 100

b.	NRIC clear text (Rec): alphanumeric 100

III.	Function call to convert Record (Rec) to Reference ID (RefID)

1.	Parameters passed from client:

a.	NRIC (Rec): alphanumeric 100

2.	Return value :

b.	NRIC hashed value: alphanumeric 100

3.	Validate NRIC and return error if NRIC is invalid format. Check whether there is already an existing NRIC upon creation. If NRIC is already existing, then there's no need to create. Initialise nonce and hash the value. After hashing is done, the system is to check if the hash value already exists, if it exist it will increment the nonce and regenerate the
