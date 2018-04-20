# QlickView
Files for reporting system

iclpartocc:
LOAD 
       BPARTNER as PARTNER,
       DELETED, 
       ROLE
FROM
[m:\Никитин\qvd\ICLPARTOCC.qvd]
(qvd)
Where DELETED <> 'X';

left join

BUT000:
LOAD
		PARTNER,
	    PERSNUMBER
FROM
[m:\Никитин\qvd\BUT000.qvd]
(qvd);

join

TICL301T:
LOAD 
       ROLE, 
       NAME
FROM
[m:\Никитин\qvd\TICL301T.qvd]
(qvd);

join

BUT020:
LOAD
		PARTNER,
		ADDRNUMBER
FROM
[m:\Никитин\qvd\BUT020.qvd]
(qvd);

join

ADRC:
LOAD
		ADDRNUMBER
			
FROM
[m:\Никитин\qvd\ADRC.qvd]
(qvd);

join

ADR6:
LOAD
		ADDRNUMBER,
		PERSNUMBER,
		SMTP_ADDR,
		SMTP_SRCH
			
FROM
[m:\Никитин\qvd\ADR6.qvd]
(qvd);

join

ADR2:
LOAD
		ADDRNUMBER,
		PERSNUMBER,
		R3_USER
			
FROM
[m:\Никитин\qvd\ADR2.qvd]
(qvd);
