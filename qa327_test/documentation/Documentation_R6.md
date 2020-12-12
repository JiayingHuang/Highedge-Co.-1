| Test Name                         | Test Features                                                                            | Nature of Failure                     | Error Classification           | Action Taken                                                                                                                                                                   |
|-----------------------------------|------------------------------------------------------------------------------------------|---------------------------------------|--------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| FrontEndBuyTest.test_name_format  | Ticket name has to be alphanumeric-only                                                  | Unable to run the test                | Indentation Error              | Correct all the indentation mistake in this unit test                                                                                                                          |
| FrontEndBuyTest.test_name_format  | Ticket name has to be alphanumeric-only                                                  | Element {#message_b} was not present  | Unexpected Assertion Failure   | Correct id #message_d of method buy_post in frontend.py to #message_b                                                                                                          |
| FrontEndBuyTest.test_quantity     | Ticket quantity has to be between 0 and 100                                              | Element {#message} was not present    | Unexpected Assertion Failure   | Correct the indentation of method buy_post in frontend.py, where if-statement for quantity and required price should be the nested-if of if-statment for checking ticket exist |
| FrontEndBuyTest.test_exist_enough | Ticket name has to be exist and it has enough ticket quantity to meet user's requirement | Element {#message} was not present    | Unexpected Assertion Failure   | Calculate an certain quantity that will not exceed the current balance and put into positive check                                                                             |
| FrontEndBuyTest.test_balance      | User's current balance can meet the required ticket price                                | Element {#message_b} was not present  | Unexpected Assertion Failure   | Create a new ticket that has different price and quantity                                                                                                                      |