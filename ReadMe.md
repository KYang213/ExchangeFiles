
Customer DOREEN FLAGG 09526-31006 states that when she called in 3 times that she was not able to speak with an agent she called from 508) 612-5270 at 12:09pm 12:15pm and 12:21PM. 

----

AMI_DEFAULT: 145,,No,0,202567,204027,Goto,NLMenu2040
AMI_NIGM: 145,,No,0,202567,204026,Goto,NLMenu2040
AMI_MASE: 145,,No,0,202567,204028,Goto,NLMenu2040
AMI_NANE: 145,,No,0,202567,204028,Goto,NLMenu2040

# FlowID_IVRXferReason:ICMXferReason,CallIntent,CallIntent_Details,XferMsg,AgentXfer
2040_AMI: AGENT_XFER,AMI,AMI,AgentXfer,TRUE
2040_AMI_DEFAULT: AGENT_XFER,AMI,AMI,AgentXfer,TRUE
2040_AMI_NIGM: AGENT_XFER,AMI,AMI,AgentXfer,TRUE

----------------
https://jira.prod.nationalgrid.com/browse/AIMCJ-1814, CUSTOM_IVR_CALL_SUMMARY


IVR.150 added new tag HEAT_PUMP to 2025 along with a new confirmation message.
Sending the callers to 2040 with new messages 204029, 204030



goto 2040
confirmation 
202435 You're calling about heat pump rates, right?  Say yes or no.


If MASE, NANE, BOSG, CLOG or ESSG
204029: Good news! If you use a heat pump to heat your home, you may qualify for a new, lower electric delivery rate. This seasonal rate runs from November 1 through April 30 and can help you save on energy costs during the colder months. Not enrolled yet? No problem—you can find more information at ngrid.com forward slask heatpumprate
Else
204030: There are not any heat pump rate discounts at this time in your area.


202435 = You're calling about heat pump rates, right?  Say yes or no.
204029 = Good news! If you use a heat pump to heat your home, you may qualify for a new, lower electric delivery rate. This seasonal rate runs from November 1 through April 30 and can help you save on energy costs during the colder months. Not enrolled yet? No problem—you can find more information at ngrid.com/heatpumprate
204030 = There are not any heat pump rate discounts at this time in your area.

----------------


HEAT_PUMP_DEFAULT: 146,,No,0,202435,204030,Goto,NLMenu2040
HEAT_PUMP_MASE: 146,,No,0,202435,204029,Goto,NLMenu2040
HEAT_PUMP_NANE: 146,,No,0,202435,204029,Goto,NLMenu2040
HEAT_PUMP_BOSG: 146,,No,0,202435,204029,Goto,NLMenu2040
HEAT_PUMP_CLOG: 146,,No,0,202435,204029,Goto,NLMenu2040
HEAT_PUMP_ESSG: 146,,No,0,202435,204029,Goto,NLMenu2040


2040_AMI_MASE: AGENT_XFER,AMI,AMI,AgentXfer,TRUE
2040_AMI_NANE: AGENT_XFER,AMI,AMI,AgentXfer,TRUE
2040_HEAT_PUMP_DEFAULT: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE
2040_HEAT_PUMP_MASE: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE
2040_HEAT_PUMP_NANE: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE
2040_HEAT_PUMP_BOSG: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE
2040_HEAT_PUMP_CLOG: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE
2040_HEAT_PUMP_ESSG: AGENT_XFER,Billing,HEAT_PUMP,AgentXfer,TRUE