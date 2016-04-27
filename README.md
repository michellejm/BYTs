# BYTs

##Corpus of Spanish/English Bilingual Youth Texts (BYTs)##

This corpus includes 44,597 messages sent by Spanish/English bilingual youth in New York City. It was part of the data collection for "Literacies of Bilingual Youth: A profile of bilingual academic, social, and txt literacy." For more information about this project, visit www.byts.commons.gc.cuny.edu. These files are encrypted. Please contact Michelle A. McSweeney at mjohnson2@gc.cuny.edu or the Second Language Acquisition Lab at the Graduate Center at CUNY slal@gc.cuny.edu with your name, affiliation, and a 1-2 sentence description of your research for the password. 

##Messages##

The messages in this corpus were downloaded directly from participants' phones by creating a history of all of their text messages and downloading the archive. Participants signed two consent forms for this and had to enter their passcode to allow access. The messages have been anonymized first computationally and then they were hand masked by two independent researchers. There are 44,500 messages in the corpus, including spam, automated messages, and mass messages from participants’ cellphone carriers.

###Fields in the Messages Table###

* **Msg_ID**: Each message has a unique identifier that begins with the letter, M

* **Usr_ID**: Each user has a unique identifier that begins with the letter, U. This indicates who donated the messages. See the Send information to determine who wrote the message. 

* **Conv_ID**: Each conversation has a unique identifier in order to keep continuous exchanges by two people intact. The purpose for this is conversation analysis. C000 is not a conversation, this code was used for mass messages and alerts. C999 is unidentifiable as a conversation though it was sent by an individual. 

* **Rel_ID**: When possible, the relationship between the people is indicated. 
	* friend: friend
	* casual: engaged in a casual sexual relationship
	* significant other: engaged in an ongoing romantic relationship
	* rel: non-immediate relative
	* sib: sibling
	* parent: parent
	
* **Gender**: When possible, the gender of the receiver is indicated

* **Message**: The message contents.

* **Date**: When available from the metadata, the date the message was sent is included. When the date was not recoverable, 1/1/00 is used.

* **Time**: When available from the metadata, the time the message was sent is included. When the time was not recoverable, 12:00:00AM is used.

* **Sent**: Whether the donator sent or received the message.

###Fields in the Demographics Table:###

* **Usr_ID**: See Above
* **Gender**: Self reported gender, only male (m) or female (f) were reported
* **Age**: Age range, either 17-19 or 20-22
* **Birthplace**: Country of birth
* **AOA**: Age of Arrival to the United States (if frequently moved, the first age is listed)
* **Phone_Type**: Participants wrote in their phone type, only Android and iPhones were used
* **Phone_Settings**: The language settings (not necessarily the keyboard) En = English, Sp = Spanish

##Fields in the Languages Table:##

* **Msg_ID**: See Above
* **Likely_Language**: Smarter result for this corpus
* **Language**: Result from stop words tagging
* **Confidence**: Number of words identified from reported language compared to all identifiable words

##Fields in the POS Table:##

* **Msg_ID**: See Above
* **Tags**: The result of computationally tagging all the messages based on the likely language result from POS tagging.

##Masked Items##

'd' indicates how many characters, including spaces and punctuation were in the masked item. For example, 234-567-8900 is masked as [NUMBER, 12] whereas 2345678900 is masked as [NUMBER, 10]

* **Numbers**: [NUMBER, 'd'] Numbers include any number that could be linked to one individual. Phone numbers, heights, weights, shoe sizes, etc. were removed, but time of day was preserved. 
* **Emails**: [EMAIL, 'd'] 
* **Places**: [PLACE, 'd'] Places include addresses or partial addresses, street names, directions, train stations, sports and music venues, names of libraries, schools, community centers, and event spaces
* **Names**: [NAME, 'd'] Names includes proper names, i.e., first and last names, diminuitive forms of names, pet names and relationship-specific terms of endearment
* **Websites**: [WEB]
* **Other** [SCRIPT] words written in unrenderable text, rarely used


###Emojis###

Emojis are encoded as [EMO, 'd'], there is another table in this package that replaces these characters with either unicode or bytes or the actual image. Because of the encoding and decoding processes, there are mistakes in this correlation. Therefore the emoji data should not be treated as preliminary data. Please contact Michelle McSweeney if you plan to work with emojis. 

