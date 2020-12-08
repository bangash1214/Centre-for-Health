# Centre-for-Health

dim message
dim number

set objFile=CreateObject("Scripting.FileSystemObject").OPenTextFile("number.txt",1)
do while not objFile.AtEndOfStream
number=objFile.ReadLine()
	message=URLEncode("https://www.youtube.com/watch?v=VHyGqsPOUHs")
	set shell=WScript.CreateObject("WScript.Shell")
	shell.run("https://web.whatsapp.com/send?phone="&number&"&text="&message)
	WScript.sleep(8000)
	shell.SendKeys "{ENTER}"
	WScript.sleep(4000)
	shell.SendKeys "^w"
Loop
objFile.close


Public Function URLEncode( StringVal )
  Dim i, CharCode, Char, Space
  Dim StringLen
  StringLen = Len(StringVal)
  ReDim result(StringLen)

  Space = "+"
  'Space = "%20"

  For i = 1 To StringLen
    Char = Mid(StringVal, i, 1)
    CharCode = AscW(Char)
    If 97 <= CharCode And CharCode <= 122 _
    Or 64 <= CharCode And CharCode <= 90 _
    Or 48 <= CharCode And CharCode <= 57 _
    Or 45 = CharCode _
    Or 46 = CharCode _
    Or 95 = CharCode _
    Or 126 = CharCode Then
      result(i) = Char
    ElseIf 32 = CharCode Then
      result(i) = Space
    Else
      result(i) = "&#" & CharCode & ";"
    End If
  Next
  URLEncode = Join(result, "")
End Function

## Inspiration: Meet Wazeera from Tribal Area of Pakistan. 

45 years old diabetes patient
Doctors recommended that she should perform aerobic exercise regularly. Aerobic activity bouts should ideally last at least 10 min, with the goal of ∼30 min/day or more, most days of the week for adults with type 2 diabetes.
But limited opportunities, restrictions on going outside of homes, culture and religion not allow her physical activities in her village. 
She and several other placing them at increased risk of non-communicable diseases (NCDs) including diabetes, heart disease and cancer.

## Background and Rationale

A growing middle-income population of young women in Pakistan rural areas experience limited opportunities for physical activity.
Diabetes affects around 17 to 19pc of Pakistanis, with approximately 35.3 million diabetics, or one out of six of the adult population of the country.  Dawn 2018 Report
Non-communicable diseases (NCDs) rates in Pakistan are significantly on the rise.

##  Problem of Focus
A growing middle-income population of young women in my hometown experience limited opportunities for physical activity placing them at increased risk of non-communicable diseases (NCDs) including diabetes, heart disease and cancer. 


## What it does

WhatsApp Chatbot channel run by women, for women to provide free convenient fitness classes in Pashto through a train-the-trainer model in Parachinar.

What does it do? Daily send a fitness video by WhatsApp chatbot channel directly to women by female instructors. 


## How I built it

Using Whatsapp Chatbot tool 'Lobster' to arrange online fitness classes in local language Pashto for the fitness of women to prevent them from non-communicable diseases (NCDs. Pakistan's first whatsapp chatbot in local language Pashto for women fitness classes.
 

## Challenges I ran into
The crucial scale of non-communicable diseases (NCDs in Parachinar with a model scalable to other rural areas of Pakistan.


## Accomplishments that I'm proud of
Winner of National SDGs Hackathon Organized by Code for Pakistan and  National Ignite Funds August 2017


## What I learned
simple solutions and high value with skilled, experienced and committed team can bring changes in the health sector of Pakistan. 


## What's next for Cetre for Health
We have plan to Initial operate it Parachinar tribal area with the support of Seed Money/Donor to launch Proof of Concept with a model scalable to other rural areas of Pakistan to teach women, Moms into Fitness is here to help women achieve their fitness goals and prevent them from non-communicable diseases (NCDs. We need Operational Funding, Partnerships and Networking opportunity to implement our project.


Whatsapp Chatbot process for Fitness Classes. #CodeForPakistan #Telenor  
