#This code is a part of the inventory project front side.

##Equipment:
component for creation an equipment item, load data from server for selectors, checks if inserted data is unique

##Equipment card:
component for listing equipment data in a card format

##Create qr-code from exist
Creating component from existing inventory number (select for checking)  or you can insert your own version


##ile qr-creation
component for creation a docx file from the passed file with inventory numbers.
If there are inventory numbers without equipment data, there will be a suggestion for user to create missing equipment
or to skip this step. Finally you get the docx file with all the qr-codes (3 in the each row)

## Filter service
A filter near to equipment, users, department handbooks, with dynamic parameters. Allow to reuse it in different places.
As a result will show list of cards with desired info.

## Http service
Service with api library and methods for getting, sending and modifying data.


## Custom stepper (for step-by-step obj creation)

### Stepper
Component with the html stepper view and actions delegation to the service. Placed in the bottom of the page
gets info about how much tabs and so on.

Has 3 parts
Main - Stepper
Basic methods for initing, step forward\back, and finish.

### StepTab  
usual stepper. Include all the elements with class 'tab'
### BigTab 
stepper for sub-pages. All elements with class 'big-tab'



