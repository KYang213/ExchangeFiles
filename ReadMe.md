
IVR Ticket: INC23688832 / 2025111420740 Customer states that when she called in 3 times that she was not able to speak with an agent 



----------------
https://jira.prod.nationalgrid.com/browse/AIMCJ-1814, CUSTOM_IVR_CALL_SUMMARY

### 2025-12 release 
#### NGAIMSBusinessServices_v2.0.5
SIT: 10/29/25 UAT: 11/13/25 PROD: 12/03/25

- updated the TTS text for 802001



### 2025-12 release 
#### NGAIMSMain_v3.0.12
SIT:10/29/25 UAT:11/13/25 PROD:12/02/25

- Tuning Grammar Updates Set 2:
	- AIMCJ-1720	(IVR.137) Grammar improvement recommendations were presented in Phase 1b, 2 and 3 tuning.
					This batch will include Payment Options, Billing Summary, Payment Plans, Account Update, 
					Billing Plans, Route Request, Meter Read, Service Orders and Start Stop Service VUIs. 43 grammar updates.
				
- Make Payments:
	- AIMCJ-1727	(IVR.138) Lower the confirmation threshold from 70 to 50 for CSS Pay Past Due (3083) and CSS Pay Total Due (3084)

- FAQ/Outage/Billing Plans: 
	- AIMCJ-1734	(IVR.139) Prompt changes for CSS Plan Start (4120), Help Paying (1825), Flickering Lights (1330) based on Tuning.

- FAQ:
	- AIMCJ-1741	(IVR.140) Prompt changes for CSS Already Have Plan (3410), Retail Access Program (1863)
	- AIMCJ-1797	(IVR.149) Updating the prompting for High Bill (1820)
	
- Payment Options:
	- AIMCJ-1748	(IVR.141) Adding bill summary to the menu (3720).

- Payment Plans:
	- AIMCJ-1755	(IVR.142) Add “help me with something else” to let callers go back to the NL (3450DM).
	- AIMCJ-1762	(IVR.143) Add MakePayment as a hidden option and have it confirm always (3470DM).

- Billing Plans:
	- AIMCJ-1770	(IVR.144) Consider adding make a payment and payment arrangements to the prompting.
	- AIMCJ-1790	(IVR.147) Adding make a payment as a hidden option.

-Meter Read:
	- AIMCJ-1776	(IVR.145) Change the order of 6100 to put hear instructions at the beginning.  Put as a hidden option and send the 
					callers to hear the instructions in 6201.
				
- Outage:
	- AIMCJ-1783	(IVR.146) Updating the handling for 1260 and removing module 1250.

- TTS: outage and payment options

- [AIMCJ-1814](https://jira.prod.nationalgrid.com/browse/AIMCJ-1814): CUSTOM_IVR_CALL_SUMMARY: added AcctNumber column (need to remove AcctLast4 in next release)
- IVR.150: added new tag HEAT_PUMP to 2025 along with a new confirmation message.
Sending the callers to 2040 with new messages 204029, 204030
- bug fix: fixed IVR.124 bug (IVR does not transfer the call when asking agent 2nd times in the NL). modified the audio for 202504 and 202551
