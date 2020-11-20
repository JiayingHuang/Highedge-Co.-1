| Test Name                               | Tested Feature                                               | Nature of Failure           |                                                    |                                                           |
| --------------------------------------- | ------------------------------------------------------------ | --------------------------- | -------------------------------------------------- | --------------------------------------------------------- |
| test_password_same_negative             | Password and password2 have to be exactly the same           | Unexpected Register Success | Error in testing code, wrong assert implementation | Change assert implementation                              |
| test_email_password_complexity_negative | Email, password, password2 all have to satisfy the same required as defined in R1 | Unexpected Register Success | Error in testing code, wrong assert implementation | Change assert implementation                              |
| test_not_loggedin                       | If the user has not logged in, show the user registration page | Unexpected Redirect Failure | Error in testing code, wrong assert parameter      | change assert parameter from "registration" to "Register" |
| test_formatting_error                   | For any formatting errors, redirect back to /login and show message '{} format is incorrect.'.format(the_corresponding_attribute) | Unexpected Register Failure | Error in frontend code, wrong message outputted    | Change error message format                               |
| test_email_exist                        | If the email already exists, show message 'this email has been ALREADY used' | Unexpected Register Success | Error in frontend code, wrong message outputted    | Change error message format                               |