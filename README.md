**Project AD + Group policy**

Requirements:

![](media/image1.png){width="6.5in" height="4.935416666666667in"}

Solution

1-Create Windows server machine and edit the next

![](media/image2.png){width="6.5in" height="1.89375in"}

1.1-Static ip:

![](media/image3.png){width="6.5in" height="3.4090277777777778in"}

1.2-TimeZone: Cairo

1.3-Machine name: PDC

![](media/image4.png){width="6.5in" height="2.2152777777777777in"}

2-To make the Machine domain controller, Need to Install AD and promote
it as a domain controller

![](media/image5.png){width="6.547221128608924in"
height="3.008865923009624in"}

![](media/image6.png){width="6.5in" height="2.5840277777777776in"}

![](media/image7.png){width="6.5in" height="2.597916666666667in"}

![](media/image8.png){width="6.5in" height="2.625in"}

Add Active directory domain service

![](media/image9.png){width="6.5in" height="4.638888888888889in"}

![](media/image10.png){width="6.5in" height="4.615972222222222in"}

![](media/image11.png){width="4.417283464566929in"
height="1.458536745406824in"}

Promote this server as a domain controller

![](media/image12.png){width="6.5in" height="4.756944444444445in"}

![](media/image13.png){width="6.5in" height="4.768055555555556in"}

![](media/image14.png){width="6.5in" height="4.774305555555555in"}

![](media/image15.png){width="6.5in" height="4.745833333333334in"}

![](media/image16.png){width="6.5in" height="4.729861111111111in"}

![](media/image17.png){width="6.5in" height="4.7756944444444445in"}

Install

![](media/image18.png){width="6.5in" height="2.3979166666666667in"}

- Creating HR,IT , Sales OU's

![](media/image19.png){width="6.5in" height="4.434027777777778in"}

![](media/image20.png){width="6.167527340332459in"
height="2.59411198600175in"}

![](media/image21.png){width="3.5212718722659666in"
height="2.4699529746281716in"}

- Users HR: Mohamed zohdy, Salma Mohamed

- Users IT: Moatz Yousef, Ahmed nabil

- Users Sales: Mahaa ahmed , Alaa kamel

![](media/image22.png){width="6.5in" height="3.4944444444444445in"}

![](media/image23.png){width="6.5in" height="3.54375in"}

![](media/image24.png){width="5.789640201224847in"
height="2.677983377077865in"}![](media/image23.png){width="6.506450131233596in"
height="2.403898731408574in"}

![](media/image25.png){width="6.5in" height="3.7993055555555557in"}

![](media/image26.png){width="6.5in" height="3.8159722222222223in"}

![](media/image27.png){width="5.771639326334208in"
height="4.823590332458442in"}

![](media/image28.png){width="4.917352362204724in"
height="0.625087489063867in"}

![](media/image29.png){width="5.709130577427821in"
height="4.959025590551181in"}

![](media/image30.png){width="5.74169072615923in"
height="3.8039665354330707in"}

![](media/image31.png){width="5.898174759405074in"
height="3.948536745406824in"}![](media/image30.png){width="5.758043525809274in"
height="4.02951990376203in"}

Add users to groups

![](media/image32.png){width="6.5in" height="3.4618055555555554in"}

![](media/image33.png){width="6.5in" height="2.0458333333333334in"}

![](media/image34.png){width="6.5in" height="1.3395833333333333in"}

![](media/image35.png){width="6.5in" height="1.8090277777777777in"}

![](media/image36.png){width="6.5in" height="2.4347222222222222in"}

Moving to Windows 10 client

![](media/image37.png){width="6.5in" height="3.170138888888889in"}

Ip 192.168.1.40

DNS 192.168.1.2

![](media/image38.png){width="6.5in" height="2.191666666666667in"}

From advanced system settings

![](media/image39.png){width="6.5in" height="3.292361111111111in"}

![](media/image40.png){width="2.9379101049868765in"
height="1.7294083552055992in"}

![](media/image41.png){width="6.5in" height="2.227777777777778in"}

- Add IT group as a local admin

Making a script

![](media/image42.png){width="1.083484251968504in"
height="1.3856102362204725in"}

![](media/image43.png){width="6.5in" height="0.775in"}

So now when the scripts run on This OU, the IT-Group will be local
admins

Note : There's no user word in the script

net localgroup administrators \"exam\IT-Group\" /add

![](media/image44.png){width="6.5in" height="4.432638888888889in"}

![](media/image45.png){width="6.5in" height="3.2888888888888888in"}

![](media/image46.png){width="4.531882108486439in"
height="4.875680227471566in"}

- Show only fonts in HR

> ![](media/image47.png){width="6.5in" height="3.3055555555555554in"}

![](media/image48.png){width="6.5in" height="0.9277777777777778in"}

![](media/image49.png){width="6.5in" height="2.8854166666666665in"}

Prevent access to command prompt

![](media/image50.png){width="6.5in" height="3.004166666666667in"}

Disable all the storages

![](media/image51.png){width="6.5in" height="1.4958333333333333in"}

People who doesn't get inhert to this GPO

To remove Properties from context menu

![](media/image52.png){width="6.5in" height="1.0604166666666666in"}

![](media/image53.png){width="6.5in" height="3.2041666666666666in"}

Need to make history password=3

Complex password with min 6 letters

Password changes every 60 days

![](media/image54.png){width="5.386167979002624in"
height="6.5946708223972in"}

![](media/image55.png){width="5.302823709536308in"
height="6.61550634295713in"}

![](media/image56.png){width="5.396586832895888in"
height="6.625925196850393in"}

![](media/image57.png){width="5.594530839895013in"
height="6.636342957130359in"}

![](media/image58.png){width="5.584113079615048in"
height="6.8134503499562555in"}

Account lock duration 30mins

![](media/image59.png){width="5.677876202974629in"
height="6.646760717410324in"}

![](media/image60.png){width="6.5in" height="4.565972222222222in"}

Author: bishoy maged

MCSA Project
