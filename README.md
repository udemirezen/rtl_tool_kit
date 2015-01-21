# rtl_tool_kit

PHONE VERSION http://youtu.be/0jC_Gypt03Q

USB MODEM DEMO https://www.youtube.com/watch?v=TCQQ0zFjzZI

About me & app

Created this app to have everything in one place for gsm debugging:)

Only programming in python for a couple of weeks so code is messy and I'm by no means a super programmer.

Ths app wouldn't be possible without the work of Poitr https://github.com/ptrkrysik/gr-gsm for creating the gsm-receiver program to capture and dump the data needed for this app to work so I'd like to thank him.

WHAT HARDWARE DO YOU NEED?

1. ubuntu 14.04 lts or whatever runs gr-gsm

2. A cheap rtl dongle from ebay http://cdn.instructables.com/FTN/NZVE/H1KHAOBZ/FTNNZVEH1KHAOBZ.MEDIUM.jpg

3. A usb dongle modem (search ebay for 3g usb dongle) This modem has to be able to use PDU mode (most do) The Modem I'm using for demos is Hauwei E173
4. Some phones work as a usb modem samsung in particular, I'm using Samsung Pocket neo GT-5310 running Android V 4.1.2.

Usb modem is more accurate as a tmsi sniffer becuase it stores the delivery reports on the sim card and the timestamps are used from these reports. The phone doesnt do this at the moment so I create one when I send each sms.

WHAT CAN I DO WITH THIS APP?

1. you can get imsi tmsi and key of the device connected to your pc.

2. you can send silent/flash sms

3. you can connect/match tmsi to a mobile number if target is on the same BTS and in GSM900/2G mode.

    BUTTONS
    
    2G MODE = puts dongle in 2G mode
    
    GQRX = runs gqrx
    
    Get Freq = get currect freq from gqrx and set in the paramaters box for airprobe/gr-gsm
    
    KAL = starts kal on option you set from drop down box.
    
    The rest are pretty self explanitory
    
    Also have airprobe version which runs airprobe with extracted key so you can see data in wireshark live rather than     having to create a bin file then convert it to a cfile.
    
Msg Count = how many sms to send

Sms Send Delay = how many seconds to send each sms

Del Report Delday = stop recording after x amount of seconds the app has time to get delievery reports back(not needed for manual mode)

FUTURE CODE

1. start stop app when key changes for airprobe so you have the right key to decode sms data.

2. create an android app to send sms and create timestamps for people that havent got a modem (not silent sms app just normal sms for a person you know and what to get tmsi)

3. Connect Kraken to get key programmattically(not sure yet if its possible but would be nice) not live data of course.

4. wait for Poitr/gr-gsm to add decoding block so gr-gsm and be used for debugging like the airprobe version can with this app with the kc on other timeslots 2S etc.

CODE COMMING SOON     
Getting out hardcoded stuff and cleaning up code.
