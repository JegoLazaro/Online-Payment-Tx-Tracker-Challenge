# Online-Payment-Tx-Tracker-Challenge
Web application which simulates an online payment transaction tracker.

When a client requests for the root path, i.e. /, the server should display views/index.hbs

The web application accepts three inputs - a name, a reference number, and an amount. When the user submits the form, the web application first checks if all fields are filled.

Upon clicking the submit button, if at least one of the form fields is not filled-up, display the error message Fill up all fields. No need to highlight the fields

The web application then saves the values in the database, then display the values in views/index.hbs (Links to an external site.). Use views/partials/card.hbs (Links to an external site.) to render the <div> for each transaction.
  
  
  Each transaction may be removed using the X button on the upper right of the <div>. Upon clicking the X button, the web application deletes the transaction from the database, then removes the corresponding <div> of the transaction from views/index.hbs (Links to an external site.). This operation should be done without refreshing the page.
  
  If the current value in the refno text field IS IN THE DATABASE:

Change the background color of the refno text field to red.
Display the error message Reference number already in the database in the <p id="error"> element in views/index.hbs (Links to an external site.).
Disable the submit button.
Else, if the current value in the refno text field IS NOT YET IN THE DATABASE:

Change the background color of the refno text field back to #E3E3E3
Remove the error message in the <p id="error"> element in views/index.hbs (Links to an external site.).
Enable the submit button.
  
