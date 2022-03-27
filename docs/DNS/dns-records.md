﻿# DNS RECORDS

## MX Records
Your MX records are somewhat unique. While you may share MX records with a wealth of other customers, not every customer has the same MX records. When you sign up, you receive an e-mail with this subject:

`[MXroute] Important Account Information`

You need to reference this to find your MX records. If you can’t find the e-mail, you can find a copy of it here:

[Email History](https://accounts.mxroute.com/index.php?/clientarea/emails/)

This is example of what the e-mail might contain for the MX records:

    DNS MX RECORDS:
    echo.mxrouting.net (Priority 10)
    echo-relay.mxrouting.net (Priority 20)
    (These above are both record type “MX” and should have the name value set to either @ or blank, not a subdomain)

## SPF Record
Your SPF record is not as unique as your MX records. Your SPF record is a TXT DNS record at the root domain. These are basic templates for your SPF record, and you can use either one (preference, nothing more):

    “v=spf1 include:mxroute.com -all”
    “v=spf1 include:mxlogin.com -all”

## DKIM
Your DKIM key is unique per domain. You can obtain your public DKIM key in DirectAdmin under “DKIM Keys” (look in the menus on the left side). You can find a tutorial for making use of it here: [https://mxroutehelp.com/index.php/2019/08/25/set-up-dkim/](https://mxroutehelp.com/index.php/2019/08/25/set-up-dkim/)

