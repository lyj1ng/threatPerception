Signature XSS SQL Table Blind SQL Server Side Normal
Modification Injection Include
(690) (123) (662) (434) (21600)
XSS S1: r"[^<]+<[^>]+>[^<>]+<\/[^>]+>" 690 0 0 0 0
S2: r"[^&]+&[^<]+<[^>]+>[^<]+<\/[^>]+>*" 432 0 0 0 0
SQL Table Modification S1: r"[^+]+\+\*\+*" 0 123 0 0 0
S2: r"[^’]+’;\+[^;]+;\+[^\+]+\+\*\+[^’]+’*" 0 123 0 0 0
Blind SQL Injection S1: r"[^;]+;[^’]+’+[^’]+’;–*" 0 0 662 0 0
S2: r"[^’]+’\);[^’]+’[^’]+’;–*" 0 0 544 0 0
Server Side Include S1: r"[^<]*<!–#[^-]+–>*" 0 0 0 434 0
S2: r"[^<]+<!–#[^-]+-[^\/]+\/[^-]+–>*" 0 0 0 114 0
