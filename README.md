# OOAD-WEEK10 Homework
Sequence Diagram

* ภาพที่ 1 Sequence Diagram ของการยืมคืน CD/DVD ในห้องสมุด

Code

 ```
@startuml
 
Member->Authorities:Borrow 
Member--> AuthoritiesInformation Borrowing 
Authorities -> CD/DVD:In Stock?? 
"CD/DVD"--> Authorities :In Stock 
Authorities -> CD/DVD:Decrease 
Authorities -> CD/DVD:Date line 
"Authorities" -> Borrow:Save Information Borrowing 

@enduml
 ```
diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK10/blob/master/Homework/Sequence%20Diagram1.png?raw=true">


* ภาพที่ 2 Sequence Diagram ของการรับโทรศัพท์

Code

 ```
@startuml
 
title Phone call

Caller->Phone : Picks up
"Phone"--> Caller  : Dial tone
"Phone"--> Caller  : Dial 
Phone -> Recipient : Ring
"Phone"--> Caller  : Ring notification
"Recipient"--> Phone  : Picks up
"Phone"--> Caller  : Hello 
"Recipient"--> Phone  : Hello

@enduml
 ```
diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK10/blob/master/Homework/Sequence%20Diagram2.png?raw=true">



* ภาพที่ 3 Sequence Diagram ของระบบ ATM

Code

 ```
@startuml
 
title ATM  

User -> ATM : InsetCard()
User -> Keypad  : Input(PIN)
Keypad -> ATM   : [Invlid pin] Warning()
 ATM  -> Monitor : [Invlid pin] Display()
Monitor -> ATM :  [Invlid pin] Stopservice()
ATM -> Monitor : DisplayMainMenu()
User-> Keypad  : Check(balance)
ATM -> Account : Checkbalance()
Account -> Monitor : ShowBalance()


@enduml
 ```
diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK10/blob/master/Homework/Sequence%20Diagram3.png?raw=true">



* ภาพที่ 4 Sequence Diagram Shopping Online

Code

 ```
@startuml
 
title Shopping Online


User -> Computer : Open Computer
Computer-> KeyBoard  : Input(Password)
KeyBoard  -> Monitor : Show Desktop
Computer -> Webshopping :  Find and Shopping online
User  -> Webshopping : Conferm order \nand Paybills
Company -> User : Wait for Product


@enduml
 ```
diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK10/blob/master/Homework/Sequence%20Diagram4.png?raw=true">


* ภาพที่ 5 Sequence Diagram ของร้านอาหาร
Code

 ```
@startuml
 
title Restaurant

Fred;Patron  -> Bob;Waiter : Order
Bob;Waiter -> Hank;Cook  :  Order Food
Bob;Waiter -> Fred;Patron  :  Serve drinks
Hank;Cook -> Bob;Waiter : Finish cooking
Bob;Waiter -> Fred;Patron  : Serve food
Fred;Patron  -> Ranee;Cashier : Pay


@enduml
 ```
diagram

<img src="https://github.com/NATAKORNCHA/OOAD-WEEK10/blob/master/Homework/Sequence%20Diagram5.png?raw=true">



##นางสาวนฏกร เจริญธรรม รหัส 57030176 








































