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
that automates this process.

## System Architecture
The program needs to be responsible and easy to use, automating the stakeholder's processes. The Architecture is documented in my 
[Figjam file (pt-br)](https://www.figma.com/file/9nKZcNv6uewaRSzuFtdvet/Automatiza%C3%A7%C3%A3o-Lista-de-Treinamento?node-id=0-1&t=HfGqiX82cFKVv6l3-0)

Therefore, the system must satisfy the following requirements:

- Import the database
- Create DOCX file to print the labels
- Register the database in the system
- Send a personalized email with the files attached

The system will be divided in **components** - designed to do a specific task independently, with a flexible interface that will allow updates to be made without having to change the entire architecture -

