# BYTs

##Corpus of Spanish/English Bilingual Youth Texts (BYTs)##

###Messages###

The messages in this corpus were downloaded directly from participants' phones by creating a history of all of their text messages and downloading the archive. Participants signed two consent forms for this and had to enter their passcode to allow access. The messages have been anonymized first computationally and then they were hand masked by two independent researchers. There are 44,500 messages in the corpus, including spam, automated messages, and mass messages from participants’ cellphone carriers.

There is one conversation in this data set that spans the first four months of a relationship. Both contributors were participants in the study, allowing for recovery of the complete conversation. When possible, other conversations have been kept intact and the conversation has been assigned a code. The intended purpose is for discourse analysis. 

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

**Masked Items**

'd' indicates how many characters, including spaces and punctuation were in the masked item. For example, 234-567-8900 is masked as [NUMBER, 12] whereas 2345678900 is masked as [NUMBER, 10]

* **Numbers**: [NUMBER, 'd'] Numbers include any number that could be linked to one individual. Phone numbers, heights, weights, shoe sizes, etc. were removed, but time of day was preserved. 
* **Emails**: [EMAIL, 'd'] 
* **Places**: [PLACE, 'd'] Places include addresses or partial addresses, street names, directions, train stations, sports and music venues, names of libraries, schools, community centers, and event spaces
* **Names**: [NAME, 'd'] Names includes proper names, i.e., first and last names, diminuitive forms of names, pet names and relationship-specific terms of endearment
* **Websites**: [WEB]
* **Other** [SCRIPT] words written in unrenderable text, rarely used


###Emojis###

Emojis are encoded as [EMO, 'd'], there is another table in this package that replaces these characters with either unicode or bytes or the actual image. Because of the encoding and decoding processes, there are mistakes in this correlation. Therefore the emoji data should not be treated as preliminary data. Please contact Michelle McSweeney if you plan to work with emojis. 

