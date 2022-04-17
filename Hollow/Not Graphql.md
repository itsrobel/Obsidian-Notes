
- ## Chat
	- id _UUID_ [Required]
	- Message _String_ [Required]
	- Id From _UUID_ [Required]
	- Id To _UUID_ [Optional] __if Direct__
	- date _Date_ [Required]
	- space _UUID_ [Optional] __if Space__
	
- ## Chat Space
	- id _UUID_ [Required]
	- Name _String_ [Required]
	- Owner _UUID_ [Required]
	- Users _List_ [User n, User n+1 , User n+....]

- ## User
	- id _UUID_ [Required]
	- Username _String_ [Required]
	- First Name _String_  [Hidden, Optional]
	- Last Name _String_ [Hidden, Optional]
	- Email _String_ [Hidden, Required]
	- Age _Date_ [Hidden, Optional] 
	- Gender _String_ [Hidden] 
	- Location _List_ [Hidden] [ long , lat ]
	- Spaces _List_ [Hidden] __ref to [Space Users] list __
	
- ## Doctor
	- Id _UUID_ [Required]
	- First Name _String_ [Required]
	- Last Name _String_ [Required]
	- Email _String_ [Required]
	- Age _Date_ [Required, Optional] 
	- Gender _String_ [Hidden] 
	- Location Of Office _List_ [Hidden, Required] [ long , lat ]
	- Spaces _List_ [Hidden] __ref to [Space Users] list __
	
	
	
	
