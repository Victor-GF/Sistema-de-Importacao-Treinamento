# Sistema de Importacao Treinamento
This system will automate some manual and repetitive tasks, so that it can be performed quickly and free of human errors. 

## Stakeholder context
My team is responsible for setting up work equipment for new employees. When the training takes place, the responsible department sends us a database in Excel 
Spreadsheet format with the information of the new employees, so we start the following process:

- Download the worksheet "ListaTreinamento.xlsx" from the email, it will contain employee data such as name, date of birth and others
- Format cell values, removing spaces before the word, special characters like "@*-_"
- Create a DOCX file to print labels for each employee's equipment
- Convert the XLSX file to a JSON, so that it can be sent to the server in a registration request in the system
- Email the formatted spreadsheet and labels to the other collaborators on the team

After all this process we can finally start preparing the equipment. We have a time-consuming routine that may have human errors, so there is a need for a system 
that automates this process, aiming at speed and credibility.

## Initial Software Requirements
- Input the database file from the user
- Format all values and save it to a new file
- Convert the new file to JSON format and request to the Web Service to register the data
- Create a DOCX file for printing the labels
- Email the formatted database and labels to the other collaborators

All this requirements are documented in my [Figjam file (pt-br)](https://www.figma.com/file/9nKZcNv6uewaRSzuFtdvet/Automatiza%C3%A7%C3%A3o-Lista-de-Treinamento?node-id=0-1&t=HfGqiX82cFKVv6l3-0)
